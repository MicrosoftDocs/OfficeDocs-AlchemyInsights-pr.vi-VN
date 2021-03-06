---
title: Khắc phục sự cố giao thức OAuth 2,0 và kết nối OpenID
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037693"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Khắc phục sự cố giao thức OAuth 2,0 và kết nối OpenID

Để giải quyết các vấn đề về OAuth 2,0 và kết nối OpenID, hãy thực hiện các bước được đề xuất sau đây:

Tham khảo các bài viết sau đây có liên quan đến cấu hình và khắc phục sự cố các giao thức OAuth 2,0 và kết nối OpenID:

- [Nền tảng Microsoft Identity và dòng mã ủy quyền OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -bài viết này mô tả cách chương trình trực tiếp với **dòng mã Grant (pkce)** trong ứng dụng của bạn, sử dụng bất kỳ ngôn ngữ nào.
- [Microsoft Identity Platform và dòng chứng danh máy khách OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -bài viết này mô tả cách chương trình trực tiếp chống lại **dòng chứng danh máy khách** trong ứng dụng của bạn.
- [Microsoft Identity Platform và OAuth 2,0 thông tin đăng ký mật khẩu của chủ sở hữu tài nguyên](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) -bài viết này mô tả cách chương trình trực tiếp chống lại **dòng điện ropc** trong ứng dụng của bạn.
    - Nền tảng Microsoft Identity chỉ hỗ trợ ROPC cho Azure AD đối tượng thuê, chứ không phải cho các tài khoản cá nhân. Điều này có nghĩa là bạn phải sử dụng điểm cuối dành riêng cho đối tượng thuê **https://login.microsoftonline.com/{TenantId_or_Name}) (** hoặc điểm cuối của **tổ chức** .
    - Các tài khoản cá nhân được mời đến một đối tượng thuê Azure AD không thể sử dụng ROPC.
    - Các tài khoản không có mật khẩu không thể đăng nhập thông qua máy tính cá nhân. Đối với kịch bản này, chúng tôi khuyên bạn nên sử dụng một dòng khác cho ứng dụng của bạn, thay vào đó.
    - Nếu người dùng cần phải sử dụng [xác thực đa yếu tố (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) để đăng nhập vào ứng dụng, họ sẽ bị chặn.
    - ROPC không được hỗ trợ trong các kịch bản [liên kết nhận dạng hỗn](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) hợp (ví dụ, Azure AD và adfs được dùng để xác thực các tài khoản tại cơ sở). Nếu người dùng có toàn trang được chuyển hướng đến nhà cung cấp căn cước tại chỗ, Azure AD không thể kiểm tra tên người dùng và mật khẩu đối với nhà cung cấp căn cước đó. Tuy nhiên, [thông qua xác thực](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) được hỗ trợ với ropc.
    - Một ngoại lệ cho kịch bản liên kết nhận dạng hỗn hợp sẽ là những điều sau: chính sách khám phá bản cái của trang chủ với bộ **xác thực Allowcloudpasswordđược** đặt thành **True** sẽ cho phép các dòng của ropc để làm việc cho người dùng được liên kết khi mật khẩu tại cơ sở được đồng bộ trên điện toán đám mây. Để biết thêm thông tin, hãy xem [bật xác thực ROPC trực tiếp của người dùng liên kết cho các ứng dụng kế thừa](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft Identity Platform và OAuth 2,0 tại-danh nghĩa-của dòng](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) -bài viết này mô tả cách trực tiếp lên chương trình đối với **dòng đã thay mặt-của (Obo)** trong ứng dụng của bạn.
- [Microsoft Identity Platform và giao thức kết nối OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -bài viết này cho biết cách thực hiện giao thức kết nối OpenID độc lập với ngôn ngữ và mô tả cách gửi và nhận thư http mà không cần sử dụng bất kỳ thư viện nguồn mở nào của Microsoft.

**Thẻ truy nhập**

[Thẻ truy nhập Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -tìm hiểu cách API của bạn có thể xác thực và sử dụng các tuyên bố bên trong mã thông báo Access. Tất cả tài liệu trong bài viết này, ngoại trừ khi ghi chú, chỉ áp dụng cho các thẻ được phát hành cho các API mà bạn đã đăng ký. Nó không áp dụng cho các thẻ được phát hành cho các API Microsoft thuộc sở hữu, cũng không thể dùng thẻ này để xác thực cách Microsoft Identity Platform sẽ phát hành thẻ cho API bạn tạo ra.

**Cấu hình ứng dụng**

Các [hạn chế về chuyển hướng URI (URL trả lời) và các hạn chế](https://docs.microsoft.com/azure/active-directory/develop/reply-url) -tìm hiểu cách đặt cấu hình URI chuyển hướng của bạn (URL trả lời). Một URI chuyển hướng hoặc URL trả lời, là vị trí mà máy chủ ủy quyền gửi cho người dùng sau khi ứng dụng đã được ủy quyền thành công và cấp mã ủy quyền hoặc mã thông báo truy nhập. Máy chủ ủy quyền gửi mã hoặc mã thông báo cho URI chuyển hướng; Vì vậy, điều quan trọng là bạn đăng ký vị trí chính xác như là một phần của quy trình đăng ký ứng dụng.

**Cung cấp ứng dụng**

[Hướng dẫn: phát triển và cung cấp kế hoạch cho một điểm cuối Scim](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) -bài viết này mô tả cách xây dựng một điểm cuối của Scim và tích hợp với dịch vụ cung cấp thông báo.



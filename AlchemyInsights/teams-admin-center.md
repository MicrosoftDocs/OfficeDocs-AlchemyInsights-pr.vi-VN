---
title: Trung tâm quản trị nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826401"
---
# <a name="teams-admin-center"></a>Trung tâm quản trị nhóm

Tìm hiểu về quản lý nhóm với [Trung tâm quản trị nhóm](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Nếu bạn không thể truy nhập vào Trung tâm quản trị nhóm, vui lòng kiểm tra các mục sau đây:

- Xác nhận rằng bạn đã cho phép các [địa chỉ IP của Office 365 và URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) phù hợp trên mọi thiết bị chu vi (tường lửa, v.v.) hoặc trong các quy tắc tường lửa trên máy cục bộ của bạn.
- Xác nhận rằng bạn đang sử dụng đăng nhập để truy nhập vào cổng thông tin quản trị nhóm khớp với tên người dùng của bạn được liệt kê trong [cổng thông tin quản trị Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Nếu người dùng không xuất hiện trong Trung tâm quản trị nhóm, vui lòng kiểm tra như sau:

- Bạn đã tạo người dùng hoặc giấy phép đã gán trong 24 giờ qua không? Vui lòng đảm bảo bạn chờ ít nhất 24 giờ trước khi mở một vé hỗ trợ.
- Xác minh bạn đã gán giấy phép thích hợp?
- Nếu bạn có một Active Directory tại chỗ, hãy xác minh rằng [giá trị của Msrtcpc-PrimaryUserAddress hoặc địa chỉ SIP trong trường ProxyAddresses trong Active Directory địa phương của bạn là duy nhất và định dạng khớp với](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**tên** người dùng từ [trung tâm quản trị Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Nếu bạn dự định giữ lại triển khai Skype for Business Server và có người dùng lưu trữ tại cơ sở và trực tuyến: Hãy làm theo các **nhóm "thiết lập kết hợp với nhóm và Skype for Business Online"** trong Pa-nen điều khiển máy chủ Skype for Business của bạn và di chuyển người dùng trực tuyến.

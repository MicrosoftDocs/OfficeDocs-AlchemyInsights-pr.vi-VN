---
title: Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779073"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Xác định hoạt động quy tắc hộp thư đến trong Nhật ký kiểm tra

Bạn có thể sử dụng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật của Microsoft 365 để xem các sự kiện về quy tắc hộp thư đến (tạo, sửa đổi và xóa bỏ quy tắc hộp thư đến).

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).

2. Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.

3. Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** .

4. Bên dưới **hoạt động của hộp thư Exchange**, hãy xác minh trường **hoạt động** được đặt là **mới-inboxrule tạo/chỉnh sửa/bật/tắt quy tắc hộp thư đến**.

5. Bấm **Tìm kiếm**.

Trong kết quả, hãy chọn một bản ghi kiểm tra. Trong phần thông tin chi tiết, hãy bấm **xem thêm thông tin**. Thông tin về thiết đặt quy tắc hộp thư đến được hiển thị trong trường **tham số** .

Để biết thêm thông tin, hãy xem [xác định nếu người dùng đã tạo một quy tắc hộp thư đến](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)

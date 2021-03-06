---
title: Các sự cố khi đăng nhập vào ứng dụng Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833037"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Khắc phục các ứng dụng Microsoft 365 "mô-đun nền tảng tin cậy của máy tính của bạn không hoạt động đúng"

Để khắc phục lỗi này, hãy thử làm như sau:

- Cài đặt các bản cập nhật mới nhất cho [Windows](https://support.microsoft.com/help/4027667/windows-10-update) và [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Xóa](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) thông tin xác thực Office bằng trình quản lý chứng danh Windows.<br/>
    **Lưu ý:** Các đường dẫn đăng ký cho Office 2016 đã thay đổi thành 16,0. (Ví dụ: \Software\Microsoft\Office\16.0\Common\Identity\)
- Hãy thử [quy trình khôi phục người dùng](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) để khắc phục lỗi mô-đun nền tảng tin cậy (TPM).
- Đặt EnableADAL = 0 bằng cách dùng các bước sau đây:  
    1. Bấm chuột phải vào nút bắt đầu của Windows, chọn **chạy**, nhập **regedit**, rồi chọn **OK**.
    2. Chọn **có** để cho phép trình soạn thảo sổ đăng ký thực hiện thay đổi đối với thiết bị của bạn.
    3. Trong trình soạn thảo sổ đăng ký, hãy thêm một giá trị DWORD của **Enableadal** với một thiết đặt của **0** dưới HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Để biết thêm thông tin, hãy xem các [vấn đề về kết nối trong đăng nhập sau khi cập nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
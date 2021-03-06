---
title: công cụ xuất khám phá điện tử
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814610"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Bạn không thể cài đặt hoặc chạy công cụ xuất khám phá điện tử?

Nếu bạn không thể cài đặt hoặc chạy công cụ xuất khám phá điện tử để tải xuống kết quả tìm kiếm, hãy kiểm tra những điều sau đây:
  
- Máy tính bạn đang sử dụng đáp ứng các trang trước:

  - 32-hoặc 64-bit phiên bản Windows 7 và các phiên bản mới hơn

  - Microsoft .NET Framework 4.7.

  - Một trình duyệt được hỗ trợ:

  - Microsoft Edge

    Hay

  - Internet Explorer 10 và các phiên bản mới hơn

    Các trình duyệt khác, chẳng hạn như Google Chrome và Mozilla Firefox không được hỗ trợ.

- Tổ chức của bạn có thể kết nối với điểm cuối trong Azure, là **\* . blob.Core.Windows.net** (ký tự đại diện trình bày một mã định danh duy nhất cho công việc xuất khẩu của bạn).

- Bạn đã gán vai trò xuất trong &amp; Trung tâm tuân thủ bảo mật của Microsoft 365. Theo mặc định, vai trò này chỉ được gán cho nhóm vai trò trình quản lý khám phá điện tử. Xem mục [gán quyền khám phá](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)điện tử.

Để biết thêm thông tin, hãy xem [xuất kết quả tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Nếu bạn đang xuất nhiều hơn 100K hộp thư, bạn sẽ cần sử dụng PowerShell sau đây để tải xuống các kết quả xuất:  [xuất kết quả từ hơn 100k hộp thư](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
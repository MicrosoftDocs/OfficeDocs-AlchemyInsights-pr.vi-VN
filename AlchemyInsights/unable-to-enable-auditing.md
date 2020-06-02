---
title: 2419-không thể kích hoạt kiểm tra
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510450"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="1d879-102">Không thể cho phép kiểm tra hợp nhất</span><span class="sxs-lookup"><span data-stu-id="1d879-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="1d879-103">Khi bạn cố gắng kích hoạt kiểm tra hợp nhất cho tổ chức của bạn, bạn có thể nhận được lỗi tương tự như sau:</span><span class="sxs-lookup"><span data-stu-id="1d879-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="1d879-104">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="1d879-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="1d879-105">[Kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="1d879-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="1d879-106">Chạy lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="1d879-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="1d879-107">Đợi 60 phút cho cài đặt trước có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="1d879-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="1d879-108">Chạy lệnh sau trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1d879-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="1d879-109">Để biết thêm thông tin, hãy xem bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="1d879-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="1d879-110">Kết nối với Exchange Online PowerShell sử dụng xác thực nhiều yếu tố</span><span class="sxs-lookup"><span data-stu-id="1d879-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="1d879-111">Bật hoặc tắt tìm kiếm Nhật ký kiểm tra</span><span class="sxs-lookup"><span data-stu-id="1d879-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)

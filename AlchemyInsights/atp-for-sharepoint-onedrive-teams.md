---
title: ATP cho SharePoint, OneDrive và Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508434"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="30651-102">ATP cho SharePoint, OneDrive và Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="30651-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="30651-103">Hãy làm theo các bước sau để bật bảo vệ khỏi mối đe dọa nâng cao:</span><span class="sxs-lookup"><span data-stu-id="30651-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="30651-104">Truy [https://protection.office.com](https://protection.office.com) cập và đăng nhập bằng tài khoản quản trị viên hoặc bảo mật toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="30651-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="30651-105">Trong ngăn điều hướng bên trái trong **quản lý mối đe dọa**, chọn **Policy** \> **tệp đính kèm an toàn**chính sách.</span><span class="sxs-lookup"><span data-stu-id="30651-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="30651-106">Chọn **bật ATP cho SharePoint, OneDrive và Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="30651-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="30651-107">[Tạo một chính sách cảnh báo hoạt động](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) để nhận thông báo khi chúng tôi phát hiện các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="30651-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="30651-108">Để có hướng dẫn đầy đủ, xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="30651-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="30651-109">**Lưu ý**: theo thiết kế, ATP không quét tất cả các tệp duy nhất trong SharePoint Online, OneDrive for Business hoặc Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="30651-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="30651-110">Các tệp được quét không đồng bộ bởi một quy trình sử dụng hoạt động chia sẻ, hoạt động của khách và tín hiệu mối đe dọa để xác định các tệp độc hại.</span><span class="sxs-lookup"><span data-stu-id="30651-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="30651-111">Để biết thêm thông tin, xem [chủ đề](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)này.</span><span class="sxs-lookup"><span data-stu-id="30651-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>

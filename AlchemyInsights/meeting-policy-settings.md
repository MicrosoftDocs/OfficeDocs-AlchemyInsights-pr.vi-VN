---
title: Thiết đặt chính sách cuộc họp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376904"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="45219-102">Quản lý chính sách cuộc họp trong Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="45219-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="45219-103">Chính sách cuộc họp được sử dụng để kiểm soát các tính năng sẵn có để gặp gỡ những người tham gia cuộc họp theo lịch trình của người dùng trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="45219-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="45219-104">Một số tính năng của chính sách cuộc họp có thể không được thực hiện trong Trung tâm quản trị teams (chúng được gắn nhãn "đến sớm" trong tài liệu).</span><span class="sxs-lookup"><span data-stu-id="45219-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="45219-105">Trong trường hợp này, hoặc nếu bạn nhận được lỗi như "chúng tôi không thể cập nhật chính sách ngay bây giờ nhưng hãy thử lại sau" trong Trung tâm quản trị Microsoft teams, chúng tôi khuyên bạn nên sử dụng PowerShell để tạo hoặc sửa đổi các chính sách cuộc họp của teams.</span><span class="sxs-lookup"><span data-stu-id="45219-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="45219-106">Để biết thêm thông tin về chính sách cuộc họp, hãy xem các tài nguyên sau:</span><span class="sxs-lookup"><span data-stu-id="45219-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="45219-107">Để tìm hiểu về cách tạo chính sách, thực hiện thay đổi và gán người dùng cho chính sách, hãy xem [quản lý chính sách cuộc họp trong teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="45219-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="45219-108">Để thực hiện thay đổi chính sách bằng cách sử dụng lệnh ghép ngắn PowerShell, hãy xem [tổng quan về nhóm PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="45219-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="45219-109">Bạn cần sử dụng [Skype dành cho doanh nghiệp PowerShell mô-đun](https://www.microsoft.com/download/details.aspx?id=39366) cho các chính sách cuộc họp teams.</span><span class="sxs-lookup"><span data-stu-id="45219-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="45219-110">Đánh giá [tài liệu lệnh ghép ngắn \*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="45219-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="45219-111">**Lưu ý:** Có thể mất đến 24 giờ để thay đổi chính sách có hiệu lực đối với người dùng.</span><span class="sxs-lookup"><span data-stu-id="45219-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="45219-112">Bạn có thể không thể thực hiện thay đổi cho chính sách mới được tạo ngay lập tức; đợi 4 giờ và cố gắng sửa đổi một chính sách mới được tạo ra một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="45219-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="45219-113">Nếu bạn vẫn gặp sự cố, hãy thử PowerShell.</span><span class="sxs-lookup"><span data-stu-id="45219-113">If you're still having problems, try PowerShell.</span></span>  
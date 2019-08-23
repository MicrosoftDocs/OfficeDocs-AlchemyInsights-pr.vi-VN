---
title: Đồng bộ hóa Profile
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554355"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="1997e-102">Khi làm thay đổi cấu hình của mình đồng bộ ứng dụng hồ sơ người dùng SharePoint?</span><span class="sxs-lookup"><span data-stu-id="1997e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="1997e-103">SharePoint Online sử dụng hoạt động thư mục nhập khẩu bộ đếm thời gian công việc (AD nhập khẩu) để nhập người dùng và nhóm vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="1997e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="1997e-104">Quảng cáo nhập khẩu đồng bộ các thay đổi từ các cửa hàng thư mục trực tuyến SharePoint để ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="1997e-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="1997e-105">Những thay đổi này được xử lý theo lô.</span><span class="sxs-lookup"><span data-stu-id="1997e-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="1997e-106">Việc đếm thời gian chạy cho đến khi các thay đổi được đồng bộ hóa.</span><span class="sxs-lookup"><span data-stu-id="1997e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1997e-107">Thời gian công việc để chạy phụ thuộc vào số lượng thay đổi để xử lý.</span><span class="sxs-lookup"><span data-stu-id="1997e-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="1997e-108">Một số lượng lớn các thay đổi mất nhiều thời gian.</span><span class="sxs-lookup"><span data-stu-id="1997e-108">A large number of changes takes longer.</span></span> <span data-ttu-id="1997e-109">Thỏa thuận cấp độ dịch vụ (SLA) nói rằng một sự thay đổi cho người dùng trong thư mục trực tuyến SharePoint sẽ được phản ánh trong ứng dụng hồ sơ người dùng trong 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="1997e-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="1997e-110">Thông tin thêm về đồng bộ hồ sơ người dùng SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1997e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  


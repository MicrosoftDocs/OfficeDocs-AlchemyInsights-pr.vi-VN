---
title: Gỡ cài đặt hoặc loại trừ teams khỏi cài đặt Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344259"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="514af-102">Gỡ cài đặt hoặc loại trừ teams khỏi cài đặt Office mới hoặc hiện tại</span><span class="sxs-lookup"><span data-stu-id="514af-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="514af-103">Microsoft teams hiện đã được đưa vào như một phần của Office 365 ProPlus, Office 365 Business và Office cho Mac.</span><span class="sxs-lookup"><span data-stu-id="514af-103">Microsoft Teams is now included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="514af-104">Sử dụng [công cụ triển khai Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) để loại trừ teams khỏi cài đặt Office mới.</span><span class="sxs-lookup"><span data-stu-id="514af-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="514af-105">Để *gỡ cài đặt* nhóm khỏi thiết bị chạy Windows, xem [dỡ cài đặt Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="514af-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="514af-106">Để làm sạch Microsoft teams từ nhiều máy mục tiêu hoặc người dùng, xem [triển khai Microsoft teams làm sạch](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="514af-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="514af-107">Sử dụng tuỳ chọn [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) để ngăn Microsoft teams cài đặt tự động với Office.</span><span class="sxs-lookup"><span data-stu-id="514af-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="514af-108">Sử dụng tùy chọn [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *trước khi teams được cài đặt*, để ngăn Microsoft teams tự khởi động sau khi cài đặt.</span><span class="sxs-lookup"><span data-stu-id="514af-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="514af-109">Nếu bạn đang sử dụng Office cho Mac, hãy xem [cài đặt Microsoft teams trên máy Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="514af-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>
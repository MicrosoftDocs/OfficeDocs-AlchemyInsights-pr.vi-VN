---
title: Không thể xóa bỏ các mục trong SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019605"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f1ec6-102">Không thể xóa các mục</span><span class="sxs-lookup"><span data-stu-id="f1ec6-102">Unable to delete items</span></span>

- <span data-ttu-id="f1ec6-103">Các chính sách duy trì có thể gây ra điều này, bạn cần tắt hoặc loại trừ giữ tương ứng đang gây ra sự cố này.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f1ec6-104">Sau khi một chính sách duy trì hoặc giữ được loại bỏ, có thể mất tới 24 giờ để thay đổi có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="f1ec6-105">Đảm bảo rằng không có thiết lập [chính sách duy trì](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) trên mục.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="f1ec6-106">Site có thể vượt quá giới hạn dung lượng lưu trữ, tăng [hạn ngạch trang](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) và xóa mục đó.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="f1ec6-107">Đảm bảo mục không được [kiểm](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) xuất cho một người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="f1ec6-108">Cuối cùng, người quản trị có thể sử dụng các [mẫu và thực hành SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) chứa một thư viện của các lệnh PowerShell cho phép bạn thực hiện các hành động quản lý phức tạp chẳng hạn như buộc xóa các mục bướng bỉnh.</span><span class="sxs-lookup"><span data-stu-id="f1ec6-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f1ec6-109">Loại bỏ tệp PNP</span><span class="sxs-lookup"><span data-stu-id="f1ec6-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f1ec6-110">Loại bỏ thư mục PNP</span><span class="sxs-lookup"><span data-stu-id="f1ec6-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f1ec6-111">Loại bỏ mục danh sách PNP</span><span class="sxs-lookup"><span data-stu-id="f1ec6-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f1ec6-112">Loại bỏ danh sách PNP</span><span class="sxs-lookup"><span data-stu-id="f1ec6-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f1ec6-113">Loại bỏ trường PNP (cột)</span><span class="sxs-lookup"><span data-stu-id="f1ec6-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)
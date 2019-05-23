---
title: Không thể xoá mục trong SharePoint hoặc OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057800"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="1cb17-102">Không thể xoá bỏ khoản mục</span><span class="sxs-lookup"><span data-stu-id="1cb17-102">Unable to delete items</span></span>

<span data-ttu-id="1cb17-103">Có vấn đề xóa mục?</span><span class="sxs-lookup"><span data-stu-id="1cb17-103">Having issues deleting items?</span></span>

- <span data-ttu-id="1cb17-104">Luôn chắc chắn rằng bạn có [quyền phù hợp](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) để xóa mục hoặc có một [bộ sưu tập quản lý](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) cố gắng loại bỏ các mục.</span><span class="sxs-lookup"><span data-stu-id="1cb17-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="1cb17-105">Đảm bảo rằng có không phải là một thiết lập [chính sách lưu giữ](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) trên mặt hàng đó.</span><span class="sxs-lookup"><span data-stu-id="1cb17-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="1cb17-106">Bảo đảm hàng không [kiểm tra](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) đến người dùng khác.</span><span class="sxs-lookup"><span data-stu-id="1cb17-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="1cb17-107">Cuối cùng, người quản trị có thể sử dụng [SharePoint Patterns và thực tiễn](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) chứa một thư viện của PowerShell lệnh cho phép bạn thực hiện các hoạt động quản lý phức tạp như buộc xóa mục bướng bỉnh.</span><span class="sxs-lookup"><span data-stu-id="1cb17-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="1cb17-108">Loại bỏ tệp PNP</span><span class="sxs-lookup"><span data-stu-id="1cb17-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="1cb17-109">Loại bỏ cặp PNP</span><span class="sxs-lookup"><span data-stu-id="1cb17-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="1cb17-110">Loại bỏ các mục danh sách PNP</span><span class="sxs-lookup"><span data-stu-id="1cb17-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="1cb17-111">Xoá danh sách PNP</span><span class="sxs-lookup"><span data-stu-id="1cb17-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="1cb17-112">Loại bỏ các PNP trường (cột)</span><span class="sxs-lookup"><span data-stu-id="1cb17-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)
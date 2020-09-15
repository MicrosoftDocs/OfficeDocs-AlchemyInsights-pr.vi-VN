---
title: Khắc phục sự cố truy nhập thư bị từ chối
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691705"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="10c83-102">Khắc phục sự cố truy nhập thư bị từ chối</span><span class="sxs-lookup"><span data-stu-id="10c83-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="10c83-103">Nếu bạn nhận được một truy nhập bị từ chối thư khi tìm cách duyệt một site SharePoint Online, vui lòng xem các bài viết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="10c83-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="10c83-104">**Thêm và cấp giấy phép cho người dùng**</span><span class="sxs-lookup"><span data-stu-id="10c83-104">**Add and License the user**</span></span>

<span data-ttu-id="10c83-105">Đảm bảo rằng bạn [gán giấy phép cho người dùng trong Microsoft 365 dành cho doanh nghiệp](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="10c83-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="10c83-106">**Gán quyền**</span><span class="sxs-lookup"><span data-stu-id="10c83-106">**Assign Permissions**</span></span>

<span data-ttu-id="10c83-107">Nếu người dùng đã được gán giấy phép SharePoint và vẫn nhận được một thông báo bị từ chối truy nhập, vui lòng đảm bảo họ có [cấp độ quyền thích hợp được gán](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="10c83-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="10c83-108">**Cân nhắc việc sử dụng tính năng yêu cầu truy nhập**</span><span class="sxs-lookup"><span data-stu-id="10c83-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="10c83-109">Tính năng [truy nhập yêu cầu](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) cho phép mọi người yêu cầu quyền truy nhập vào nội dung mà họ hiện không có quyền để xem.</span><span class="sxs-lookup"><span data-stu-id="10c83-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="10c83-110">**Cho phép script tùy chỉnh có thể khiến các vấn đề bị từ chối truy nhập**</span><span class="sxs-lookup"><span data-stu-id="10c83-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="10c83-111">Có một số kịch bản nhất định mà tính năng "cho phép tùy chỉnh" có thể đang trình bày một truy nhập bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="10c83-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="10c83-112">Để biết danh sách các tính năng bị ảnh hưởng, cân nhắc về bảo mật và khả năng vô hiệu hóa tính năng.</span><span class="sxs-lookup"><span data-stu-id="10c83-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="10c83-113">Vui lòng truy nhập, [cho phép hoặc ngăn chặn Script tùy chỉnh](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="10c83-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="10c83-114">Lưu ý: Nếu site OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, có thể có sự cố dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="10c83-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="10c83-115">[Kiểm tra bảng điều khiển trạng thái dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="10c83-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  


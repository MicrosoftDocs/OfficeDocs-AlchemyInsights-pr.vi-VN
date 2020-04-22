---
title: Truy cập bị từ chối khi ánh xạ ổ đĩa SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687388"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="575b1-102">Khắc phục sự cố với thư viện SharePoint ánh xạ ổ đĩa mạng</span><span class="sxs-lookup"><span data-stu-id="575b1-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="575b1-103">Khi bạn duyệt một ổ đĩa mạng bị ánh xạ, bạn có thể thấy một thông báo sau:</span><span class="sxs-lookup"><span data-stu-id="575b1-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="575b1-104">**\\Đường dẫn không thể truy cập. Bạn có thể không có quyền sử dụng tài nguyên mạng này. Liên hệ với quản trị viên của máy chủ này để tìm hiểu nếu bạn có quyền truy cập.**</span><span class="sxs-lookup"><span data-stu-id="575b1-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="575b1-105">**Truy nhập bị từ chối. Trước khi mở tệp ở vị trí này, đầu tiên bạn phải thêm trang web vào danh sách trang web đáng tin cậy của bạn, duyệt đến trang web và chọn tùy chọn để đăng nhập tự động.**</span><span class="sxs-lookup"><span data-stu-id="575b1-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="575b1-106">[Nhận trợ giúp khắc phục sự cố ổ đĩa mạng được ánh xạ](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="575b1-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="575b1-107">Ánh xạ thư viện là một ổ đĩa mạng tạm thời và được hỗ trợ chỉ trong Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="575b1-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="575b1-108">Thay vào đó, [đồng bộ hoá SharePoint tệp với khách hàng đồng bộ OneDrive mới](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) bao gồm [các tệp theo yêu cầu](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="575b1-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="575b1-109">Truy cập tất cả các tệp của bạn trong OneDrive mà không sử dụng dung lượng lưu trữ cục bộ.</span><span class="sxs-lookup"><span data-stu-id="575b1-109">Access all your files in OneDrive without using local storage space.</span></span>
  
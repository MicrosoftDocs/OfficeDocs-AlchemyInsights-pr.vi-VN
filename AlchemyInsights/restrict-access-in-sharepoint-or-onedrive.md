---
title: Hạn chế truy cập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905170"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fc1fa-102">Hạn chế truy cập trong SharePoint hoặc OneDrive</span><span class="sxs-lookup"><span data-stu-id="fc1fa-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fc1fa-p101">Trong SharePoint và OneDrive, bạn hạn chế quyền truy cập vào các mục như các tập tin, thư mục và danh sách bằng cách cấp quyền truy cập chỉ để nhóm hay cá nhân muốn có quyền truy cập. Theo mặc định, các cấp phép SharePoint được thừa hưởng từ cao lên trong hệ thống. Vì vậy một tập tin thừa hưởng các quyền của mình từ thư mục cấp phép của nó thừa hưởng từ thư viện của nó quyền thừa hưởng từ các trang web.</span><span class="sxs-lookup"><span data-stu-id="fc1fa-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="fc1fa-p102">Bạn có thể chia sẻ ở một mức độ cao hơn (chẳng hạn như bằng cách chia sẻ một trang web toàn bộ) và sau đó chia di sản thừa kế nếu bạn không muốn chia sẻ tất cả các mục trên trang web. Tuy nhiên, chúng tôi không khuyên bạn nên điều này bởi vì nó làm cho việc duy trì các điều khoản phức tạp và khó hiểu hơn trong tương lai. Dưới đây là những gì bạn có thể làm để thay thế:</span><span class="sxs-lookup"><span data-stu-id="fc1fa-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="fc1fa-109">Nếu, ví dụ, bạn muốn chia sẻ tất cả các nội dung của một thư mục ngoại trừ các tập tin một trong nó, di chuyển tệp đó đến một vị trí mới không phải là chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="fc1fa-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="fc1fa-110">Nếu bạn có 2 thư mục con trong thư mục, và bạn muốn chia sẻ một thư mục con với các nhóm A và B và cho phép chỉ group A quyền truy cập vào các thư mục con thứ hai, chia sẻ thư mục mẹ với group A và thêm nhóm B để các thư mục con đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="fc1fa-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="fc1fa-111">Dừng chia sẻ tệp hoặc cặp</span><span class="sxs-lookup"><span data-stu-id="fc1fa-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  


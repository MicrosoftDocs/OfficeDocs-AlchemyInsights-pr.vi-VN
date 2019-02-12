---
title: Tập tin mở chỉ-đọc
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 2b7f27e38412fc2a1dea46027e926c660231ed8b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903082"
---
# <a name="file-open-read-only"></a><span data-ttu-id="8f31c-102">Tập tin mở chỉ-đọc</span><span class="sxs-lookup"><span data-stu-id="8f31c-102">File open read-only</span></span>

<span data-ttu-id="8f31c-p101">Bạn có thể thấy rằng khi bạn đang mở tập tin, họ mở như chỉ-đọc. Trong một số trường hợp, đây là an toàn hơn, chẳng hạn như khi bạn đang mở tập tin từ internet và các thời điểm khác, nó có thể do một thiết lập mà có thể được thay đổi. Dưới đây là một số kịch bản mà một tập tin mở ra chỉ có đọc và một số bước bạn có thể làm để thay đổi điều đó.</span><span class="sxs-lookup"><span data-stu-id="8f31c-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="8f31c-106">**Antivirus của tôi gây ra cho họ để mở chỉ-đọc**</span><span class="sxs-lookup"><span data-stu-id="8f31c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="8f31c-p102">Một số chương trình chống vi-rút có thể bảo vệ bạn từ các tập tin có khả năng không an toàn bằng cách mở chúng chỉ-đọc. Bạn có thể cần phải kiểm tra với nhà cung cấp chống vi-rút của bạn để tìm hiểu làm thế nào để điều chỉnh các cài đặt này. BitDefender, ví dụ, có nội dung về việc thêm ứng dụng trường hợp loại trừ ở đây: [làm thế nào để thêm ứng dụng hoặc quá trình loại trừ trong Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="8f31c-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="8f31c-110">**Được các thuộc tính tệp thiết lập để chỉ đọc không?**</span><span class="sxs-lookup"><span data-stu-id="8f31c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="8f31c-p103">Bạn có thể kiểm tra các thuộc tính tệp bằng cách bấm chuột phải vào file và chọn thuộc tính. Nếu đã kiểm tra các thuộc tính chỉ đọc, bạn có thể bỏ chọn nó và nhấn OK.</span><span class="sxs-lookup"><span data-stu-id="8f31c-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="8f31c-113">**Nội dung là trong diện được bảo vệ**</span><span class="sxs-lookup"><span data-stu-id="8f31c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="8f31c-p104">Tập tin từ Internet và từ các địa điểm có khả năng không an toàn có thể chứa vi-rút, sâu, hoặc các loại khác của phần mềm độc hại có thể làm hại máy tính của bạn. Điều này cũng thường là trường hợp với file đính kèm email hoặc các tập tin bạn đã tải xuống. Để giúp bảo vệ máy tính của bạn, các tập tin từ các địa điểm có khả năng không an toàn được mở trong chế độ xem bảo vệ. Bằng cách sử dụng Protected View, bạn có thể đọc một tập tin và xem nội dung của nó trong khi làm giảm những rủi ro. Để biết thêm chi tiết về bảo vệ xem và làm thế nào để thay đổi cài đặt, xem bài viết này: [xem bảo vệ là gì?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="8f31c-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="8f31c-119">**OneDrive là đầy đủ?**</span><span class="sxs-lookup"><span data-stu-id="8f31c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="8f31c-p105">Nếu tập tin được lưu trữ trên OneDrive và dung lượng lưu trữ OneDrive của bạn là đầy đủ, bạn sẽ không thể lưu tài liệu cho đến khi bạn đang trong không gian được phân bổ của bạn. Bạn có thể kiểm tra không gian miễn phí của bạn trên OneDrive bằng cách nhấp vào biểu tượng OneDrive ở trung tâm thông báo và chọn Manage storage, hoặc bạn có thể đi đến [http://onedrive.live.com](http://onedrive.live.com), đăng nhập và lưu ý số lượng các không gian được sử dụng ở dưới bên trái của màn hình.</span><span class="sxs-lookup"><span data-stu-id="8f31c-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="8f31c-122">**Văn phòng được kích hoạt?**</span><span class="sxs-lookup"><span data-stu-id="8f31c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="8f31c-p106">Nếu văn phòng không được kích hoạt, hoặc đăng ký của bạn đã hết hạn, bạn có thể chỉ đọc giảm chức năng Mode. Thông tin về làm thế nào để kích hoạt Office, xem: [sản phẩm không có giấy phép và kích hoạt lỗi trong văn phòng](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="8f31c-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="8f31c-125">**Nếu vẫn thất bại...**</span><span class="sxs-lookup"><span data-stu-id="8f31c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="8f31c-126">Thử khởi động lại máy tính</span><span class="sxs-lookup"><span data-stu-id="8f31c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="8f31c-127">Cài đặt bản Cập Nhật Office</span><span class="sxs-lookup"><span data-stu-id="8f31c-127">Install Office updates</span></span>
    
- <span data-ttu-id="8f31c-128">Thực hiện một sửa chữa văn phòng trực tuyến</span><span class="sxs-lookup"><span data-stu-id="8f31c-128">Perform an Online repair of Office</span></span>
    


---
title: 1554 Winsock lỗi 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772463"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c3052-102">Winsock lỗi 10061</span><span class="sxs-lookup"><span data-stu-id="c3052-102">Winsock error 10061</span></span>

<span data-ttu-id="c3052-103">Mã lỗi này có nghĩa rằng Office 365 không thể thiết lập một cổng TCP (kết nối) với máy chủ mục tiêu.</span><span class="sxs-lookup"><span data-stu-id="c3052-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c3052-104">Nguyên nhân có thể nhất của lỗi này là một vấn đề với cấu hình tường lửa của bạn.</span><span class="sxs-lookup"><span data-stu-id="c3052-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c3052-105">Để khắc phục vấn đề, hãy kiểm tra các cài đặt này:</span><span class="sxs-lookup"><span data-stu-id="c3052-105">To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="c3052-106">Xác minh cấu hình tường lửa của bạn với các thông tin trong [Office 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c3052-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="c3052-107">Nếu lỗi cụ thể để bảo vệ trực tuyến trao đổi (EOP), bạn nên đã được trước đó thông báo để thay đổi [địa chỉ IP bảo vệ trực tuyến trao đổi](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c3052-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="c3052-108">Xác minh rằng nhà cung cấp dịch vụ Internet (ISP) không phải là chặn cổng.</span><span class="sxs-lookup"><span data-stu-id="c3052-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="c3052-109">Xác minh các thông minh chủ và mục tiêu máy chủ cài đặt kết nối của bạn.</span><span class="sxs-lookup"><span data-stu-id="c3052-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="c3052-110">Lưu ý rằng Office 365 không chặn *các* kết nối theo cách này.</span><span class="sxs-lookup"><span data-stu-id="c3052-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

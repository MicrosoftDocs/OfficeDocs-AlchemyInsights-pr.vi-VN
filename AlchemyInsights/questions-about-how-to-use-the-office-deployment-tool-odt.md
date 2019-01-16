---
title: Các câu hỏi về làm thế nào để sử dụng công cụ triển khai văn phòng (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320043"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="4decf-102">Các câu hỏi về làm thế nào để sử dụng công cụ triển khai văn phòng (ODT)</span><span class="sxs-lookup"><span data-stu-id="4decf-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="4decf-103">Tải về công cụ triển khai Office từ [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="4decf-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="4decf-104">Sau khi tải về các tập tin, chạy tập tin thực thi tự giải nén chứa các văn phòng triển khai công cụ thực thi (setup.exe) và một tập tin cấu hình mẫu (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="4decf-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="4decf-105">**Để loại trừ hoặc loại bỏ các sản phẩm Office 365 ProPlus từ máy tính khách hàng:**</span><span class="sxs-lookup"><span data-stu-id="4decf-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="4decf-p101">Khi cài đặt Office 365 ProPlus, bạn có thể loại trừ sản phẩm cụ thể. Để làm như vậy, hãy làm theo các bước để cài đặt văn phòng với ODT, nhưng bao gồm các yếu tố ExcludeApp trong tập tin cấu hình của bạn. Ví dụ, tập tin cấu hình này sẽ cài đặt tất cả các sản phẩm Office 365 ProPlus trừ nhà xuất bản:</span><span class="sxs-lookup"><span data-stu-id="4decf-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="4decf-109">Tổng quan về công cụ triển khai văn phòng</span><span class="sxs-lookup"><span data-stu-id="4decf-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


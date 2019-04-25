---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402761"
---
Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry. 
  
|**Khóa sổ đăng ký**|**Loại hình**|**Giá trị**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Để biết thêm chi tiết, hãy xem [Sử xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL được kích hoạt theo mặc định trong Office 365 ProPlus và Office 2016. > dịch vụ máy tính để bàn từ xa (RDS) trước đây được đặt tên là dịch vụ đầu cuối. 
  


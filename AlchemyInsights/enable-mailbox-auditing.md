---
title: Sử hộp thư kiểm tra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757840"
---
# <a name="enable-mailbox-auditing"></a>Sử hộp thư kiểm tra

Để kích hoạt hộp thư kiểm toán cho một người dùng hoặc một tổ chức toàn bộ các lệnh ghép ngắn sau đây phải được chạy từ xa điện vỏ:
  
 **Người dùng duy nhất**
  
Set-Mailbox - Identity "Jane Dow" - AuditEnabled $true
  
 **Tổ chức**
  
Get-Mailbox – ResultSize không giới hạn - lọc {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true
  
[Tìm hiểu thêm](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  


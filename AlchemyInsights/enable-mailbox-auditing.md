---
title: Bật kiểm tra hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506976"
---
# <a name="enable-mailbox-auditing"></a>Bật kiểm tra hộp thư

Để kích hoạt hộp kiểm tra cho người dùng hoặc một tổ chức toàn bộ các lệnh ghép ngắn sau đây phải được chạy từ xa điện vỏ:
  
 **Người dùng đơn**
  
Thiết lập hộp thư-Identity "Jane Dow"-AuditEnabled $true
  
 **Tổ chức**
  
Get-hộp thư-ResultSize không giới hạn-lọc {RecipientTypeDetails-EQ "UserMailbox"} | Thiết lập hộp thư-AuditEnabled $true
  
[Tìm hiểu thêm](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  


---
title: Các thư được gửi đến nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823809"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Các thư được gửi đến một nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên

Đảm bảo rằng tất cả các thành viên nhóm đã đăng ký nhận email. Xem [theo dõi một nhóm trong Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Để kiểm tra trạng thái thư của những thành viên đã đăng ký với email nhóm, hãy chạy lệnh sau đây trên [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Sử dụng lệnh EXO PowerShell sau đây để cấu hình tất cả các thành viên nhóm để nhận email được gửi đến nhóm Microsoft 365 trong hộp thư đến của họ:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Ví dụ:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`
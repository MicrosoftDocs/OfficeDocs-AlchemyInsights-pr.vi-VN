---
title: Đặt ClientAccessServerEnabled thành True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527415"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="9143d-102">Đặt ClientAccessServerEnabled thành True</span><span class="sxs-lookup"><span data-stu-id="9143d-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="9143d-103">Nếu bạn không thể mở thư email đã mã hóa và thay vào đó, hãy xem phần đính kèm **rpmsg** , thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="9143d-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="9143d-104">Kết nối với Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9143d-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="9143d-105">Để kết nối với Exchange Online PowerShell, bạn phải đăng nhập bằng tài khoản người quản trị toàn cầu hoặc tài khoản người quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="9143d-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="9143d-106">một.</span><span class="sxs-lookup"><span data-stu-id="9143d-106">a.</span></span> <span data-ttu-id="9143d-107">Mở Windows PowerShell, rồi chạy lệnh sau đây: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="9143d-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="9143d-108">b.</span><span class="sxs-lookup"><span data-stu-id="9143d-108">b.</span></span> <span data-ttu-id="9143d-109">Trong hộp thoại yêu cầu chứng danh của **Windows PowerShell** , hãy nhập tài khoản và mật khẩu cơ quan hoặc trường học của bạn, c.</span><span class="sxs-lookup"><span data-stu-id="9143d-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="9143d-110">Bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="9143d-110">Click **OK**.</span></span> 

2. <span data-ttu-id="9143d-111">Chạy lệnh sau đây để tạo một phiên mới:</span><span class="sxs-lookup"><span data-stu-id="9143d-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="9143d-112">một.</span><span class="sxs-lookup"><span data-stu-id="9143d-112">a.</span></span> <span data-ttu-id="9143d-113">Chạy lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="9143d-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="9143d-114">`Get-IRMConfiguration`Lệnh chạy.</span><span class="sxs-lookup"><span data-stu-id="9143d-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="9143d-115">Kiểm tra cài đặt **Clientaccessserverenabled** .</span><span class="sxs-lookup"><span data-stu-id="9143d-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="9143d-116">một.</span><span class="sxs-lookup"><span data-stu-id="9143d-116">a.</span></span> <span data-ttu-id="9143d-117">Nếu thiết đặt **Clientaccessserverenabled** được đặt là **false**, hãy chạy lệnh ghép ngắn sau đây: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="9143d-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="9143d-118">Luôn đóng phiên PowerShell với lệnh sau đây: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="9143d-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="9143d-119">Để biết thêm thông tin, hãy xem [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="9143d-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>


---
title: Cài đặt Office trên máy chủ đầu cuối-không có giấy phép
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735411"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="7c547-102">Cài đặt Office trên máy chủ đầu cuối</span><span class="sxs-lookup"><span data-stu-id="7c547-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="7c547-103">Để triển khai Office 365 ProPlus trên Windows Server sử dụng dịch vụ máy tính để bàn từ xa (RDS), trước đây có tên dịch vụ đầu cuối:</span><span class="sxs-lookup"><span data-stu-id="7c547-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="7c547-104">Bạn phải có một gói Office 365 bao gồm Office 365 ProPlus, chẳng hạn như Office 365 Enterprise E3 hoặc Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="7c547-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="7c547-105">Các gói Office 365 Business và Office 365 Business Premium không bao gồm Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="7c547-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="7c547-106">Bạn cần bật [kích hoạt máy tính dùng chung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="7c547-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="7c547-107">Nếu bạn muốn cài đặt Office 365 ProPlus trên RDS từ Trung tâm quản trị Microsoft 365, ***sử dụng cài đặt mặc định***, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="7c547-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="7c547-108">Kiểm tra những gì Office 365 kế hoạch bạn có.</span><span class="sxs-lookup"><span data-stu-id="7c547-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="7c547-109">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="7c547-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="7c547-110">Nếu cần thiết, chuyển sang một gói Office 365 khác.</span><span class="sxs-lookup"><span data-stu-id="7c547-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="7c547-111">Tìm hiểu cách</span><span class="sxs-lookup"><span data-stu-id="7c547-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="7c547-112">Nếu Office đã được cài đặt trên máy chủ RDS sử dụng bất kỳ kế hoạch Office 365 khác, dỡ cài đặt.</span><span class="sxs-lookup"><span data-stu-id="7c547-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="7c547-113">Ví dụ: bằng cách đi tới Pa \> -nen điều khiển gỡ cài đặt chương trình.</span><span class="sxs-lookup"><span data-stu-id="7c547-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="7c547-114">Dỡ cài đặt bằng cách sử dụng [Microsoft support và phục hồi](https://aka.ms/SARA-OfficeUninstall-Alchemy) hỗ trợ nếu bạn đang chạy vào vấn đề.</span><span class="sxs-lookup"><span data-stu-id="7c547-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="7c547-115">Trên máy chủ RDS, đăng nhập vào Trung tâm quản trị Microsoft 365 với tài khoản quản trị viên của bạn và [cài đặt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="7c547-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="7c547-116">Sau khi Office được cài đặt, ***không mở hoặc đăng nhập*** vào bất kỳ ứng dụng Office.</span><span class="sxs-lookup"><span data-stu-id="7c547-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="7c547-117">Trên máy chủ RDS, cho phép kích hoạt máy tính được chia sẻ bằng việc chỉnh sửa sổ đăng ký bằng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="7c547-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="7c547-118">Bấm chuột phải vào nút Windows ở góc dưới bên trái của màn hình và chọn chạy.</span><span class="sxs-lookup"><span data-stu-id="7c547-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="7c547-119">Trong ô mở, gõ **regedit**, và sau đó chọn OK.</span><span class="sxs-lookup"><span data-stu-id="7c547-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="7c547-120">Chọn có khi được nhắc để cho phép Registry Editor thay đổi thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="7c547-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="7c547-121">Trong Registry Editor, thêm một giá trị chuỗi **Sharedcomputerlicensing** với thiết đặt 1 trong HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="7c547-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="7c547-122">Trên máy chủ RDS, ***đăng nhập là người dùng cuối*** và [xác minh rằng kích hoạt máy tính dùng chung được kích hoạt cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="7c547-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="7c547-123">Để biết thêm chi tiết về điều kiện tiên quyết, hướng dẫn thiết lập và hướng dẫn cài đặt tuỳ chỉnh bằng cách sử dụng công cụ triển khai Office, hãy xem [triển khai Office 365 ProPlus bằng cách sử dụng dịch vụ máy tính để bàn từ xa](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="7c547-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="7c547-124">Để khắc phục lỗi liên quan đến kích hoạt máy tính dùng chung, vui lòng xem [khắc phục sự cố với kích hoạt máy tính dùng chung cho Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="7c547-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506868"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="6b6ff-103">Lỗi khi kích hoạt Office 2013 trên máy tính để bàn từ xa dịch vụ</span><span class="sxs-lookup"><span data-stu-id="6b6ff-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="6b6ff-104">Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="6b6ff-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="6b6ff-105">**Khoá đăng ký**</span><span class="sxs-lookup"><span data-stu-id="6b6ff-105">**Registry key**</span></span>|<span data-ttu-id="6b6ff-106">**Loại**</span><span class="sxs-lookup"><span data-stu-id="6b6ff-106">**Type**</span></span>|<span data-ttu-id="6b6ff-107">**Đáng giá tiền**</span><span class="sxs-lookup"><span data-stu-id="6b6ff-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b6ff-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="6b6ff-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="6b6ff-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="6b6ff-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="6b6ff-110">1</span><span class="sxs-lookup"><span data-stu-id="6b6ff-110">1</span></span>  <br/> |

<span data-ttu-id="6b6ff-111">Để biết thêm thông tin, xem [kích hoạt xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="6b6ff-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="6b6ff-112">ADAL được bật theo mặc định trong Microsoft 365 ứng dụng cho doanh nghiệp và Office 2016.</span><span class="sxs-lookup"><span data-stu-id="6b6ff-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="6b6ff-113">Dịch vụ máy tính để bàn từ xa (RDS) trước đây có tên là dịch vụ đầu cuối.</span><span class="sxs-lookup"><span data-stu-id="6b6ff-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  
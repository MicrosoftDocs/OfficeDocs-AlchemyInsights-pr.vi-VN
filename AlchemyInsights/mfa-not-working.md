---
title: Vấn đề với MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250187"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="cd1ea-102">Vấn đề với MFA</span><span class="sxs-lookup"><span data-stu-id="cd1ea-102">Issues with MFA</span></span>
<span data-ttu-id="cd1ea-103">Có một vài điều để kiểm tra nếu người dùng không thể đăng nhập bằng cách sử dụng nhiều yếu tố xác thực (MFA)</span><span class="sxs-lookup"><span data-stu-id="cd1ea-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cd1ea-104">Người dùng bị ảnh hưởng có thể bị chặn trong Azure Active Directory cổng.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cd1ea-105">Nếu trường hợp đó xảy ra, xác thực nỗ lực cho rằng người dùng cụ thể sẽ được tự động bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cd1ea-106">Xin vui lòng làm theo các bước trong bài viết này để bỏ chặn họ.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cd1ea-107">Nếu bỏ chặn người dùng đã không giúp đỡ hoặc không chặn người dùng bạn có thể thử đặt lại MFA cho người dùng và họ sẽ đi qua quá trình ghi danh một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cd1ea-108">Xin vui lòng làm theo các bước trong bài viết này.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cd1ea-109">Nếu đây là lần đầu tiên bạn kích hoạt MFA và người dùng của bạn là không thể đăng nhập vào trình duyệt không khách hàng chẳng hạn như Outlook, Skype, vv, có lẽ ADAL (Active Directory xác thực thư viện) không được kích hoạt trên đăng ký của bạn O365.</span><span class="sxs-lookup"><span data-stu-id="cd1ea-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cd1ea-110">Trong trường hợp này bạn sẽ cần để kết nối với Exchange Online Powershell và chạy lệnh ghép ngắn này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="cd1ea-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>
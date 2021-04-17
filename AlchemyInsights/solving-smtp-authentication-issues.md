---
title: Giải quyết các sự cố xác thực SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826437"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="0908b-102">Giải quyết các sự cố xác thực SMTP</span><span class="sxs-lookup"><span data-stu-id="0908b-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="0908b-103">Nếu bạn đang gặp phải lỗi 5.7.57 hoặc 5.7.3 khi tìm cách gửi email SMTP và xác thực bằng một máy khách hoặc ứng dụng, có một vài điều bạn nên kiểm tra:</span><span class="sxs-lookup"><span data-stu-id="0908b-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="0908b-104">Việc gửi SMTP được xác thực có thể bị vô hiệu hóa trong đối tượng thuê của bạn hoặc trên hộp thư mà bạn đang cố gắng sử dụng (kiểm tra cả hai thiết đặt).</span><span class="sxs-lookup"><span data-stu-id="0908b-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="0908b-105">Để đọc thêm, hãy xem [bật hoặc tắt trình gửi SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)được xác thực.</span><span class="sxs-lookup"><span data-stu-id="0908b-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="0908b-106">Kiểm tra xem [mặc định bảo mật Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) được bật cho đối tượng thuê của bạn hay không; Nếu được kích hoạt, xác thực SMTP bằng cách dùng xác thực cơ bản (còn được gọi là di sản; điều này sẽ sử dụng tên người dùng và mật khẩu) sẽ không thành công.</span><span class="sxs-lookup"><span data-stu-id="0908b-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>

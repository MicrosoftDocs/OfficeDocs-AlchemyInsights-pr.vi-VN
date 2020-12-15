---
title: Sửa đổi Microsoft Edge bằng cách dùng các biến dữ liệu của thư mục thay vì đường dẫn hardcoded
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679157"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="c7c45-102">Sửa đổi Microsoft Edge bằng cách dùng các biến dữ liệu của thư mục thay vì đường dẫn hardcoded</span><span class="sxs-lookup"><span data-stu-id="c7c45-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="c7c45-103">Ví dụ, trên Windows, để lưu trữ dữ liệu hồ sơ dưới dữ liệu ứng dụng cục bộ của người dùng thay vì ở vị trí mặc định, hãy đặt chính sách **Userdatadir** thành **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="c7c45-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="c7c45-104">Để tìm hiểu thêm, hãy xem [tạo các biến số thư mục dữ liệu người dùng Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span><span class="sxs-lookup"><span data-stu-id="c7c45-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>
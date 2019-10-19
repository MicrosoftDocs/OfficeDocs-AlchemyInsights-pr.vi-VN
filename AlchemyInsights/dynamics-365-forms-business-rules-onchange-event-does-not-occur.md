---
title: Dynamics 365 Forms quy định kinh doanh-quy tắc kinh doanh không bắn cho một mẫu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529041"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="0666b-102">Sự kiện Ajax xảy ra nếu trường được thay đổi lập</span><span class="sxs-lookup"><span data-stu-id="0666b-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="0666b-103">Sự kiện *Ajax* xảy ra nếu trường được thay đổi lập bằng cách sử dụng các *thuộc tính.* phương pháp [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="0666b-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="0666b-104">Nếu bạn muốn xử lý sự kiện *onChange* để chạy sau khi bạn đặt giá trị bạn phải sử dụng *thuộc tính formcontext. Data. ENTITY.* phương pháp [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) trong mã của bạn.</span><span class="sxs-lookup"><span data-stu-id="0666b-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)

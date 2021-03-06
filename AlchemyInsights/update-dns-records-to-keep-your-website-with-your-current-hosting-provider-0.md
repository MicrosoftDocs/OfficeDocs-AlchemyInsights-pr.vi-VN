---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827562"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại

1. Trong Trung tâm quản trị Microsoft 365, hãy đi đến  >  trang[tên miền](https://admin.microsoft.com/Adminportal#/Domains) thiết lập và trong danh sách tên miền, chọn tên miền mà bạn đang sử dụng cho website của bạn.

2. Chọn **+ bản ghi tùy chỉnh mới** và nhập nội dung sau đây:

  - Đối với **loại DNS** , hãy nhập: **A (địa chỉ)**

  - Đối với **tên máy chủ hoặc biệt danh**, hãy nhập các tùy chọn sau: **@**

  - Đối với **địa chỉ IP**, hãy nhập địa chỉ IP tĩnh cho trang web của bạn tại vị trí hiện tại được lưu trữ (ví dụ,: 172.16.140.1).

    Đây phải là một địa chỉ IP  *tĩnh*  cho trang web, chứ không phải địa chỉ IP  *động*  . Kiểm tra với site nơi lưu trữ website của bạn để đảm bảo rằng bạn có thể nhận được địa chỉ IP tĩnh cho trang web công cộng của bạn.

3. Chọn **lưu**.

Ngoài ra, bạn có thể tạo một bản ghi CNAME để giúp khách hàng tìm thấy website của bạn.
  
1. Chọn **+ bản ghi tùy chỉnh mới** và nhập nội dung sau đây:

  - Đối với **loại DNS** , hãy nhập: **CNAME (biệt danh)**

  - Đối với **tên máy chủ hoặc biệt danh**, hãy gõ như sau: **www**

  - Đối với **trỏ tới địa chỉ**, hãy nhập tên miền đủ điều kiện (FQDN) cho website của bạn (ví dụ, contoso.com).

2. Chọn **lưu**.

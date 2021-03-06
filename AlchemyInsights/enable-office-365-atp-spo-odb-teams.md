---
title: Bật Office 365 ATP cho tất SharePoint, OneDrive và các Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543950"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Bật Bộ bảo vệ Microsoft dành Office 365 cho SharePoint Online, OneDrive và Microsoft Teams

1. Truy nhập https://protection.office.com và đăng nhập.
2. Chọn Chính **sách quản lý mối**  >  **đe**  >  **dọa Két sắt phần đính kèm**.
3. Chọn **Bật Bộ bảo vệ cho Office 365 cho SharePoint, OneDrive và Microsoft Teams**, sau đó bấm **Lưu**.
4. (Được đề xuất) Với tư cách là người quản trị toàn cầu hoặc người quản trị SharePoint Online, hãy chạy lệnh ghép ngắn [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) với tham số **DisallowInfectedFileDownload** được đặt thành *true.*
5. (Được đề xuất) [Thiết lập cảnh báo cho các](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tệp được phát hiện.

> [!NOTE]
> Bộ bảo vệ Microsoft dành Office 365 sẽ không quét từng tệp riêng lẻ trong SharePoint Online, OneDrive hoặc Microsoft Teams. Các tệp được quét không đồng bộ, thông qua một quy trình sử dụng các sự kiện hoạt động chia sẻ và khách, cùng với tín hiệu phân tích thông minh và mối đe dọa để xác định các tệp độc hại. Xem [mục Bộ bảo vệ Microsoft Office 365 để biết SharePoint, OneDrive và Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
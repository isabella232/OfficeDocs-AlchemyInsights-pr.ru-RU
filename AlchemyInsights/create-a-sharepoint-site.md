---
title: Создание сайта SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080903"
---
# <a name="create-a-sharepoint-site"></a>Создание сайта SharePoint

Создание или управление сайтами [из активных сайтов](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) в центре SharePoint администрирования. Дополнительные сведения см. в [сайте Управление сайтами в новом центре администрирования SharePoint.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>Советы:

- Невозможно **создать** сайт с одинаковым URL-адресом существующего сайта. Если вы удалили сайт и хотите повторно использовать URL-адрес, возможно, удаленный сайт по-прежнему существует в [удаленных сайтах](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). Для повторного использования URL-адреса веб-сайт должен быть окончательно удален. Чтобы полностью удалить сайт с powershell, см. в примере [cmdlet Remove-SPSite.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)
- Некоторые пользователи могут не создать сайт. [См. в SharePoint Online.](https://docs.microsoft.com/sharepoint/manage-site-creation)
- Возможно, сайт будет застрять при **создании дольше,** чем ожидалось. Если прошло более 24 часов с тех пор, как вы впервые увидели эту проблему, зайдите в журнал билета поддержки. Во многих случаях мы уже работаем над решением. Пожалуйста, дайте нам по крайней мере 24 часа, чтобы завершить решение.

---
title: Регулирование SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048629"
---
# <a name="sharepoint-online-throttling"></a>Регулирование SharePoint Online

При попытке перейти к сайтам SharePoint или OneDrive пользователи могут получить сообщение о занятости сервера 503. 

Эта ошибка может быть вызвана регулированием в службе SharePoint. для обеспечения оптимальной производительности и надежности службы SharePoint OnlineSharePoint Online использует регулирования. Пределы регулирования количество пользовательских действий или одновременных звонков (с скриптах или программах) для предотвращения чрезмерного использования ресурсов. Если вы получите ограничением, 99% времени его из-за пользовательского кода.

Для получения дополнительных сведений об регулированиях см. [Избегайте регулирования или блокировки в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Если вы считаете, что эта ошибка не связана с регулированием, вы можете проверить, есть ли активное обслуживание клиента, перейдя в [Центр сообщений](https://portal.office.com/adminportal/home#/MessageCenter).

 Наконец, убедитесь, что вы посещаете страницу [работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth) , чтобы проверить, какие рекомендации и происшествия могут возникать.


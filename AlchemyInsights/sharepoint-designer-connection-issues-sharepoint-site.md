---
title: SharePoint Проблемы с подключением конструктора
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942038"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Проблемы с подключением конструктора 

Если SharePoint конструктор испытывает проблемы с подключением к SharePoint сайтам, попробуйте следующие распространенные решения.

Шаг 1. Убедитесь, что SharePoint Designer 2013 обновляется с [помощью SharePoint Designer Пакет обновления 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и обновления от 2 августа 2016 г. для SharePoint Designer [2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Шаг 2. Очистить локальные файлы кэша:

1. Закрыть SharePoint Designer 2013.

2. На локальном компьютере удалите все файлы, найденные в каждой из следующих папок.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы узнать, работает ли она.

Шаг 3. [Включить современную проверку подлинности Office 2013 г. на Windows устройствах.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Шаг 4. Администраторам  необходимо разрешить настраиваемый скрипт в параметрах центра администрирования SharePoint, чтобы разрешить подключение SharePoint конструктора. Дополнительные [сведения см. в тексте Разрешить](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) или запретить настраиваемый скрипт.



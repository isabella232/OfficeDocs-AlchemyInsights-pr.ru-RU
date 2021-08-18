---
title: Read-Only для обслуживания при попытке использования SharePoint или OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329461"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only для обслуживания при попытке использования SharePoint или OneDrive

Пользователи могут получать сообщение **Только** для чтения для обслуживания при попытке SharePoint или OneDrive для одного из следующих сценариев. 

-   Плановая или активная работа по обслуживанию.  Проверьте их, переехав в [Центр сообщений.](https://portal.office.com/adminportal/home#/messagecenter)
-   Инцидент с активной службой с высоким приоритетом, который может иметь место. Проверьте, есть ли какие-либо советы и инциденты, перенавигав [службу "Здоровье".](https://portal.office.com/adminportal/home#/servicehealth)
-   Небольшой сценарий восстановления автозаживления, который может произойти из-за непредвиденных событий на серверах, которые могут длиться менее 30 минут или около того. 
    
    Для этих незначительных восстановлений нет центра сообщений или службы, но вы должны вернуться к нормальной жизни очень скоро.

В очень редких случаях мы заметили, что один из трех перечисленных выше сценариев был причиной, и служба была восстановлена, но кэш браузера пользователей не был очищен.

Перед переходом на сайт попробуйте очистить кэш браузера.

1. В браузере Microsoft Edge выберите **Параметры,** а затем выберите **конфиденциальность и безопасность.**
2. В **статье Clear browsing** выберите **выберите, что нужно очистить.**
3. Выберите **файлы Cookie и сохраненные данные веб-сайта** и выберите **Clear**.

**Примечание.** Эти действия могут отличаться при использовании других браузеров, таких как Mozilla Firefox или Google Chrome.

**Примечание.** Другой вариант заключается в том, чтобы открыть SharePoint или OneDrive в новом окне InPrivate.
---
title: Надстройка Teams для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940688"
---
# <a name="teams-add-in-for-mac"></a>Надстройка Teams для Mac

Чтобы устранить проблему с отсутствующей надстройкой Teams для пользователей операционной системы компьютеров Mac, выполните следующие действия:

**Шаг 1.** При локальном применении гибридной среды Exchange (версия 2016 с накопительным пакетом обновления 3 или более поздняя версия) используйте средство Test-HMA.ps1, чтобы подтвердить правильность настройки гибридной современной проверки подлинности. Дополнительные сведения см. в разделе [Проверка настройки гибридной современной проверки подлинности в Outlook для iOS и Android](https://aka.ms/TestHMAEAS).  

**Примечание**. Используйте формат адреса UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)), а не домен\имя_пользователя. Выполняйте это даже для пользователей с почтовыми ящиками Exchange Online.

**Шаг 2.** Попросите пользователя перейти в раздел **Средства** > **Учетные записи**... в Outlook для Mac, а затем найти и выбрать учетную запись. Убедитесь, что имя пользователя указано в формате UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)).

**Шаг 3.** Подтвердите, что пользователь является лицензированным пользователем Microsoft Teams. Пользователь должен использовать подписку на Office 365 для Mac версии 16.24 или более поздней.
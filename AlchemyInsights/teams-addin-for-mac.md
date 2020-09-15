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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670341"
---
# <a name="teams-add-in-for-mac"></a>Надстройка Teams для Mac

Чтобы устранить проблему с отсутствующей надстройкой Teams для пользователей операционной системы компьютеров Mac, выполните следующие действия:

**Шаг 1.** При локальном применении гибридной среды Exchange (версия 2016 с накопительным пакетом обновления 3 или более поздняя версия) используйте средство Test-HMA.ps1, чтобы подтвердить правильность настройки гибридной современной проверки подлинности. Дополнительные сведения см. в разделе [Проверка настройки гибридной современной проверки подлинности в Outlook для iOS и Android](https://aka.ms/AA980zq).  

**Примечание**. Используйте формат адреса UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)), а не домен\имя_пользователя. Выполняйте это даже для пользователей с почтовыми ящиками Exchange Online.

**Шаг 2.** Попросите пользователя перейти в раздел **Средства** > **Учетные записи**... в Outlook для Mac, а затем найти и выбрать учетную запись. Убедитесь, что имя пользователя указано в формате UPN (например, [имя_пользователя@contoso.com](mailto:username@contoso.com)).

**Шаг 3.** Подтвердите, что пользователь является лицензированным пользователем Microsoft Teams. Пользователь должен использовать подписку на Office 365 для Mac версии 16.24 или более поздней.
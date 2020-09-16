---
title: Удаление закрытого канала Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730928"
---
# <a name="delete-a-teams-private-channel"></a>Удаление закрытого канала Teams

Корпорации Майкрософт известно о проблемах с удалением закрытого канала группы, если для сайта SharePoint включены политики хранения SharePoint. Разработчики Майкрософт работают над созданием решения. Тем временем можно воспользоваться следующими временными решениями для удаления закрытого канала.

**Исключите команду/семейство веб-сайтов из политики хранения Sharepoint.**

1. Перейдите на портал администрирования Office 365 и выберите **Показать все** в области навигации слева.
2. В разделе **Центры администрирования** перейдите на страницу **Безопасность и соответствие требованиям** > **Защита от потери данных** > **Политика**.
3. Определите все политики, применяемые к сайтам Sharepoint, и измените политику таким образом, чтобы сайт команды Sharepoint, содержащий закрытый канал, НЕ был включен в политику хранения.
4. Сохраните политику.
    Применение измененных параметров политики может занять до 24 часов.
    После исключения сайта можно удалить закрытый канал.  
    
***Возможно***, вам удастся удалить закрытый канал, используя Microsoft Teams на устройстве Android. 

Сведения по теме о SharePoint см. в статье [Не удается удалить элементы в SharePoint Online и в OneDrive для бизнеса](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).
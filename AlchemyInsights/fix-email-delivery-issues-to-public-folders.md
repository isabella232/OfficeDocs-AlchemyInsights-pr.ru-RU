---
title: Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677941"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту

Если внешние отправители не могут отправлять сообщения в общедоступные папки с включенной поддержкой почты, а отправители не получают сообщение об ошибке **(550 5.4.1)**, убедитесь, что домен электронной почты для общедоступной папки настроен как домен внутренней ретрансляции, а не уполномоченный домен:

1. Откройте [центр администрирования Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Перейдите в раздел **поток обработки почты** \> **обслуживаемые домены**, выберите обслуживаемый домен и нажмите кнопку **изменить**.

3. На открывшейся странице "Свойства", если для типа домена задано значение " **удостоверяющий**", измените значение на " **Внутренняя ретрансляция** " и нажмите кнопку **сохранить**.

Если внешние отправители получают сообщение об ошибке, у **которого нет разрешения (550 5.7.13)**, выполните следующую команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , чтобы просмотреть разрешения для анонимных пользователей в общедоступной папке:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Пример: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Чтобы разрешить внешним пользователям отправлять электронную почту в эту общедоступную папку, добавьте право доступа CreateItems для анонимного пользователя. Например, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.

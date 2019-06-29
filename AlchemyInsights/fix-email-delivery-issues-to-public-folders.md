---
title: Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387718"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту

Если внешние отправители не могут отправлять сообщения в общедоступные папки с включенной поддержкой почты, а отправители не могут найти сообщение об ошибке **(550 5.4.1)**, убедитесь, что домен электронной почты для общедоступной папки настроен как домен внутренней ретрансляции, а не в удостоверяющий домен:

1. Откройте [центр администрирования Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Перейдите в раздел **поток** \> обработки почты **обслуживаемые домены**, выберите обслуживаемый домен и нажмите кнопку **изменить**.

3. На открывшейся странице "Свойства", если для типа домена задано **** значение "удостоверяющий", измените значение на " **Внутренняя ретрансляция** " и нажмите кнопку **сохранить**.

Если внешние отправители получают сообщение об ошибке, у **которого нет разрешения (550 5.7.13)**, выполните следующую команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , чтобы просмотреть разрешения для анонимных пользователей в общедоступной папке:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Пример: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Чтобы разрешить внешним пользователям отправлять электронную почту в эту общедоступную папку, добавьте право доступа CreateItems для анонимного пользователя. Например, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.

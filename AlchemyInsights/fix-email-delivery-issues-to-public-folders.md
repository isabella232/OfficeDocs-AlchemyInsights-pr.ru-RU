---
title: Устранение проблем с доставкой электронной почты в общедоступные папки с поддержкой почты
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068825"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Устранение проблем с доставкой электронной почты в общедоступные папки с поддержкой почты

Если внешние отправители не могут отправлять сообщения в общедоступные папки с поддержкой почты, а отправители получают ошибку: не удалось найти **(550 5.4.1),** убедитесь, что домен электронной почты для общедоступных папок настроен как домен внутренней ретрансляции вместо авторитетного домена:

1. Откройте центр [администрирования Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Перейдите **к потоку** \> **почты принятых доменов,** выберите принятый домен, а затем нажмите **кнопку Изменить**.

3. На открываемой странице свойств, если тип домена установлен  до **"Авторитетный",** измените значение на внутреннюю ретранслятор, а затем нажмите **кнопку Сохранить**.

Если внешние отправители получают ошибку, у вас нет разрешения **(550 5.7.13),** запустите следующую команду в [Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) чтобы увидеть разрешения анонимных пользователей в общедоступных папках:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Например, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Чтобы позволить внешним пользователям отправлять электронную почту в эту публичную папку, добавьте право доступа CreateItems к пользователю Anonymous. Например, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.

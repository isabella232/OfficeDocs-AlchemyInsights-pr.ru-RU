---
title: Ошибка адресов прокси при создании общего почтового ящика
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568303"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Ошибка адресов прокси при создании почтового ящика или другого объекта с включенной электронной почтой

Если вы попытались создать объект с поддержкой электронной почты (почтовый ящик, общий почтовый ящик и т.д.) и получили ошибку "Прокси-адрес "SMTP:alias@domain.com" уже используется...", выбранный вами адрес электронной почты уже взят другим объектом с поддержкой электронной почты в организации.
  
Необходимо найти пользователя, группу, общий почтовый ящик или общедоступные папки с этим адресом электронной почты и удалить его или изменить адрес электронной почты. Затем можно создать новый объект с включенной электронной почтой с освобожденным адресом электронной почты. Чтобы найти его, используйте поиск на домашней странице. Вы также можете использовать следующую команду Exchange Online PowerShell для поиска:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Если вы не хотите удалять существующий адрес электронной почты, выберите новый адрес электронной почты для нового объекта, который вы создаете.
  
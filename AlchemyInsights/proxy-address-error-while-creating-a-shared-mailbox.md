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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062921"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Ошибка адресов прокси при создании почтового ящика или другого объекта с включенной электронной почтой

Если вы попытались создать объект с поддержкой электронной почты (почтовый ящик, общий почтовый ящик и т.д.) и получили ошибку "Прокси-адрес "SMTP:alias@domain.com" уже используется...", выбранный вами адрес электронной почты уже взят другим объектом с поддержкой электронной почты в организации.
  
Необходимо найти пользователя, группу, общий почтовый ящик или общедоступные папки с этим адресом электронной почты и удалить его или изменить адрес электронной почты. Затем можно создать новый объект с включенной электронной почтой с освобожденным адресом электронной почты. Чтобы найти его, используйте поиск на домашней странице. Вы также можете использовать следующую команду Exchange Online PowerShell для поиска:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Если вы не хотите удалять существующий адрес электронной почты, выберите новый адрес электронной почты для нового объекта, который вы создаете.
  
---
title: Отправка в качестве общедоступных папок с включенной почтой в EXO
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
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052579"
---
# <a name="sendas-mail-enabled-public-folder"></a>Почта SendAs включена в общедоступные папки

В следующем примере пользователь Джейсон назначает разрешения "Отправить как" для открытой папки с поддержкой почты NewPF1.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Подробные сведения о синтаксисах и параметрах см. в статью [Назначение разрешений "Отправить как"](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)или "Отправить от имени" для общедоступных папок с поддержкой почты.


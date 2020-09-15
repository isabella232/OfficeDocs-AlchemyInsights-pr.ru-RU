---
title: Политика общего доступа к календарю 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684243"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Ошибка политики при предоставлении общего доступа к календарю

1. В зависимости от ситуации выполните одно из следующих действий:
    - Подключение к Exchange Online с помощью удаленного сеанса PowerShell. Дополнительные сведения см. [в статье подключение к Exchange Online с помощью удаленной оболочки PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Откройте консоль управления Exchange на локальном сервере.
2. Определение политики общего доступа, назначенной пользователю. Для этого выполните следующую команду и обратите внимание на то, что возвращена политика:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Обновите политику общего доступа для пользователя. Для этого выполните следующие действия:
    - Откройте Центр администрирования Exchange
    - Щелкните элемент **Организация**, а затем дважды щелкните политику, назначенную пользователю в разделе **индивидуальный общий доступ**. Это политика, которая была возвращена на шаге 2.
    - На странице правило общего доступа выберите уровень общего доступа к календарю, который вы хотите разрешить, в разделе **Укажите, какие сведения вы хотите предоставить к совместному**использованию; Нажмите кнопку **сохранить**.

Дополнительные сведения см. в разделе ["политика не разрешает предоставление разрешений на этом уровне к одной или нескольким получателям", если пользователь пытается предоставить общий доступ к календарю](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).

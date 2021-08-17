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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091616"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Ошибка политики при совместном использовании календаря

1. Сделайте одно из следующих, если это подходит для вашей ситуации:
    - Подключение Exchange Online с помощью remote PowerShell. Дополнительные сведения см. [в Подключение Exchange Online с помощью remote PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - На локальном сервере откройте оболочку Exchange управления.
2. Определите политику общего доступа, назначенную пользователю. Для этого запустите следующую команду и обратите внимание на возвращаемую политику:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Обновление политики общего доступа для пользователя. Для этого выполните следующие действия:
    - Откройте Центр администрирования Exchange
    - Щелкните **Организацию,** а затем дважды щелкните политику, назначенную пользователю в разделе **Individual Sharing.** Это политика, которая была возвращена в шаге 2.
    - На странице Правило общего доступа выберите уровень общего доступа к календарю, который необходимо разрешить в разделе Укажите, какие сведения **вы хотите поделиться;** нажмите **кнопку Сохранить**.

Дополнительные сведения см. в разделе "Политика не позволяет предоставлять разрешения на этом уровне одному или несколько ошибок [получателя(ы)"](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)при попытках пользователя поделиться календарем.

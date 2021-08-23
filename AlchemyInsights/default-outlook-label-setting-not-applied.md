---
title: Параметр Outlook по умолчанию не применяется
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370214"
---
# <a name="default-outlook-label-setting-not-applied"></a>Параметр Outlook по умолчанию не применяется

Если параметры Outlook по умолчанию не применяются должным образом и не применяются другие метки или метки, вы можете испытывать известные проблемы (MC277818) и должны сделать один из этих 2 параметров для решения проблемы:

**Вариант 1:**

1. Перейдите в Microsoft 365 Центра >   >  **решений.**
1. Выберите **политики Метки** и выберите политику меток, которые необходимо изменить (параметр **OutlookDefaultlabel** не установлен должным образом в политике меток, о чем идет речь. Запустите **get-labelpolicy** для просмотра этого параметра, а затем выберите **политику редактирования**.
1. Выберите **Далее,** пока не увидите параметр **Применить** эту метку  по умолчанию к электронным письмам, которая  доступна, если вы выберите Требуют, чтобы пользователи применяли метку к электронным письмам и документам наследника в диалоговом окне Параметры политики.
1. В **диалоговом окне Применить метку по** умолчанию к диалоговом окне документов выберите **None** из списка выпаданий.
1. Выберите **Далее** **и Отправить,** чтобы сохранить параметры метки.

**Вариант 2:**

В Центре безопасности и соответствия требованиям [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)используйте командлет Set-LabelPolicy, чтобы изменить **OutlookDefaultlabel** на **None** на {OutlookDefaultLabel="None"}.

Запуск: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Дополнительные сведения о метки по умолчанию для Outlook см. в [Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)
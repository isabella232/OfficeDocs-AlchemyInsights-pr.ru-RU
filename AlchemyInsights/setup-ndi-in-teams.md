---
title: Включить технологию NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917320"
---
# <a name="turn-on-ndi-technology"></a>Включить технологию NDI

Для технологии NDI требуется два этапа, которые необходимо включить для пользователя:

1. Администратор клиента должен включить свойство AllowNDIStreaming в CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. После заполнения этого изменения конечный пользователь должен включить технологию NDI® для своего клиента в параметрах **> Permissions.**

Дополнительные сведения см. в [теме "Использование технологии NDI в Microsoft Teams".](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)

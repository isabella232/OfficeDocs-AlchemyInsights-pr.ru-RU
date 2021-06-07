---
title: Управление регистрацией в вебинаре
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783143"
---
# <a name="manage-webinar-registration"></a>Управление регистрацией в вебинаре

Управляйте тем, кто может регистрироваться в вебинарах Teams, с помощью команд PowerShell Teams. Сведения об установке PowerShell Teams см. в разделе [Teams PowerShell](/microsoftteams/teams-powershell-install). 

По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **EveryoneInCompany**. Чтобы разрешить регистрацию всем, в том числе анонимным пользователям, присвойте политике собраний значение **Все** с помощью команды PowerShell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Примечание**. Если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам. Дополнительные сведения и инструкции по включению этого параметра см. в статье [Управление параметрами собраний в Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.

Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).

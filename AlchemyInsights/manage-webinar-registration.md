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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798657"
---
# <a name="manage-webinar-registration"></a>Управление регистрацией в вебинаре

Управляйте тем, кто может регистрироваться в вебинарах Teams, с помощью команд PowerShell Teams. Сведения об установке PowerShell Teams см. в разделе [Teams PowerShell](/microsoftteams/teams-powershell-install). 

По умолчанию параметр *whoCanRegister* включен и ему присвоено значение **Все**. 

Если в приглашении на собрание вы не видите параметр, разрешающий регистрацию для всех пользователей, повторно запустите параметр *WhoCanRegister* со значением "Все" и подождите 24 часа. Чтобы повторно запустить параметр *WhoCanRegister*, используйте команду Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Примечание**. Если анонимное присоединение отключено в параметрах собрания, анонимные пользователи не смогут присоединяться к вебинарам. Дополнительные сведения и инструкции по включению этого параметра см. в статье [Управление параметрами собраний в Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Если вы хотите отключить регистрацию в собраниях, присвойте параметру *allowMeetingRegistration* значение **False**.

Дополнительные сведения о настройке того, кто может регистрироваться в вебинарах, см. в разделе [Настройка пользователей, которые могут регистрироваться в вебинарах](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Дополнительные сведения о параметрах Microsoft Списки см. в статье [Управление параметрами для Microsoft Списки](/sharepoint/control-lists).

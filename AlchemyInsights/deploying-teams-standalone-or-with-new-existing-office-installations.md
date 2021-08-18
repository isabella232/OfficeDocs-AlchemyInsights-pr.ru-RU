---
title: Развертывание Teams в качестве автономных или с новыми или существующими Office установками
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320135"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Развертывание Teams в качестве автономных или с новыми или существующими Office установками

Microsoft Teams теперь включена в состав  новых установок Приложения Microsoft 365 для предприятий, Приложения Microsoft 365 для бизнеса и Office для Mac. Дополнительные сведения см. в Microsoft Teams, включив новые установки [Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Кроме того, начиная с версии 1906 в current  Channel Teams будут добавлены к существующим установкам Приложения Microsoft 365 для предприятий (и Приложения Microsoft 365 для бизнеса) на устройствах, работающих Windows при обновлении существующей установки до последней версии. Дополнительные сведения [см. в дополнительных](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps) сведениях о существующих установках Office?

**Примечание.** Если вы не хотите ждать этого расписания развертывания, вы можете развернуть Teams как [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) автономный для пользователей, следуя этим инструкциям, или вы можете установить Teams для себя от [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Если ваша организация не готова к развертыванию Teams, у нас есть шаги, которые [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) можно [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) предпринять, чтобы исключить Teams из новых или существующих установок Office.  Если вы хотите Teams, но не хотите, чтобы Teams автоматически начался для пользователя после его установки, см. в Microsoft Teams от запуска автоматически [после](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)установки .

Чтобы ***удалить Teams*** устройства с Windows, см. в [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Чтобы очистить Microsoft Teams из нескольких целевых машин или пользователей, см. Microsoft Teams [развертывания очистки](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Если вы используете общие компьютеры, службы удаленного рабочего стола (RDS) или инфраструктура виртуальных рабочих столов (VDI), см. общие среды компьютера и [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)с Microsoft Teams .

Если вы используете Office для Mac, Microsoft Teams [установки на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Примечание.** После Teams устанавливается, он [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) автоматически обновляется примерно каждые две недели с новыми функциями и обновлениями качества. 
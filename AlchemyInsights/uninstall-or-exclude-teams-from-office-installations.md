---
title: Удалить или исключить Teams из установок Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827805"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Удалить или исключить Teams из новых или существующих установок Office

Microsoft Teams входит в состав Microsoft 365 Apps для предприятия, Microsoft 365 Apps для бизнеса и Office для Mac.

- Используйте [средство развертывания Office,](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) чтобы исключить Teams из новых установок Office.
- Чтобы удалить Teams *с* устройства под управлением Windows, см. в записи Удалить [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Чтобы очистить Microsoft Teams от нескольких целевых машин или пользователей, см. в записи [развертывания Microsoft Teams.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- Используйте параметр [PreventTeamsInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) чтобы не допустить автоматической установки Microsoft Teams в Office.
- Используйте параметр [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) перед установкой *Teams,* чтобы предотвратить автоматический запуск Microsoft Teams после установки.

Если вы используете Office для Mac, см. установки [Microsoft Teams на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).
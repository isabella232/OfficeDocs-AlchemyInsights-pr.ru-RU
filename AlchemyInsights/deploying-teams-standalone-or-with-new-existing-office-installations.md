---
title: Развертывание команд в автономном режиме или с помощью новых или существующих установок Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054243"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Развертывание команд в автономном режиме или с помощью новых или существующих установок Office

Microsoft Teams теперь входит в состав ***новых установок*** Office 365 профессиональный плюс, Office 365 для бизнеса и Office для Mac. Дополнительные сведения о том, [когда будет запущено приложение Microsoft Teams, будет включено в новые установки Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Кроме того, начиная с версии 1906 в месячном канале, Teams будет ***добавляться к существующим установкам*** Office 365 профессиональный плюс (и Office 365 бизнес) на устройствах под управлением Windows, когда вы обновите текущую установку до последней версии. Дополнительные сведения [о существующих установках Office](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Если вы не хотите ждать этого расписания развертывания, вы можете развернуть Teams как самостоятельный для пользователей, выполнив [указанные ниже инструкции](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) , или пользователи смогут установить Teams самостоятельно [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Если ваша организация не готова к развертыванию Teams, мы поможем предпринять действия для ***исключения Teams*** из [новых](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) или [существующих](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) экземпляров Office. Если вы хотите установить Teams, но не хотите, чтобы команда автоматически запускалась для пользователя после установки, ознакомьтесь со статьей [запретить автоматический запуск Microsoft Teams после установки](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Чтобы ***Удалить Teams*** с устройства под управлением Windows, ознакомьтесь с разделом [uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Чтобы очистить Microsoft Teams с нескольких целевых компьютеров или пользователей, ознакомьтесь с разделом [развертывание Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Если вы используете общие компьютеры, службы удаленных рабочих столов (RDS) или инфраструктуру виртуальных рабочих столов (VDI), ознакомьтесь [со статьей общие среды компьютера и VDI с Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Если вы используете Office для Mac, ознакомьтесь с разделом [Установка Microsoft Teams на компьютере Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> После установки Teams он [автоматически обновляется](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизительно каждые две недели с новыми функциями и обновлениями качества. 
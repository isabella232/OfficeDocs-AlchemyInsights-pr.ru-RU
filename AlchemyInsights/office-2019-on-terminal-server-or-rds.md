---
title: Office 2019 на сервере терминалов или RDS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: ded0f399f1688108803fbb04aaca6a88397e1f1a
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796326"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="db0b2-102">Развертывание Office 2019 для совместного использования в RDS, сервере терминалов или VDI</span><span class="sxs-lookup"><span data-stu-id="db0b2-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="db0b2-103">Если Office уже установлен на сервере RDS с помощью других планов Office, удалите его.</span><span class="sxs-lookup"><span data-stu-id="db0b2-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="db0b2-104">Например, откройте **панель** > управления,**а затем удалите программу**.</span><span class="sxs-lookup"><span data-stu-id="db0b2-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="db0b2-105">Если у вас возникли проблемы, удалите ее с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="db0b2-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="db0b2-106">Используйте средство развертывания Office (ODT) для установки Office.</span><span class="sxs-lookup"><span data-stu-id="db0b2-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="db0b2-107">Подробное описание действий приведено в разделе [Deploying Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span><span class="sxs-lookup"><span data-stu-id="db0b2-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="db0b2-108">Для активации просмотрите раздел [Обзор многопользовательской активации Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span><span class="sxs-lookup"><span data-stu-id="db0b2-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>
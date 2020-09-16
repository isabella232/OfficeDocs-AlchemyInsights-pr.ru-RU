---
title: Office 2019 на сервере терминалов или RDS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: 5454fad58411e9d86e19dfa83a1a553a2c2b05b4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47754578"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="cc91b-102">Развертывание Office 2019 для совместного использования в RDS, сервере терминалов или VDI</span><span class="sxs-lookup"><span data-stu-id="cc91b-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="cc91b-103">Если Office уже установлен на сервере RDS с помощью других планов Office, удалите его.</span><span class="sxs-lookup"><span data-stu-id="cc91b-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="cc91b-104">Например, откройте **Панель управления**,  >  **а затем удалите программу**.</span><span class="sxs-lookup"><span data-stu-id="cc91b-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="cc91b-105">Если у вас возникли проблемы, удалите ее с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="cc91b-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="cc91b-106">Используйте средство развертывания Office (ODT) для установки Office.</span><span class="sxs-lookup"><span data-stu-id="cc91b-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="cc91b-107">Подробное описание действий приведено в разделе [Deploying Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span><span class="sxs-lookup"><span data-stu-id="cc91b-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="cc91b-108">Для активации просмотрите раздел [Обзор многопользовательской активации Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span><span class="sxs-lookup"><span data-stu-id="cc91b-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>
---
title: Действия Защитника Windows в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 732b7450121f85416bb0f1868b3722899bee8194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699100"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="27aa1-102">Действия Защитника Windows в Intune</span><span class="sxs-lookup"><span data-stu-id="27aa1-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="27aa1-103">Можно использовать Intune, чтобы запускать проверку по запросу и обновлять сигнатуры вирусов в Защитнике Windows на отдельных устройствах.</span><span class="sxs-lookup"><span data-stu-id="27aa1-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="27aa1-104">После успешного запуска удаленного действия это действие записывается в журнале событий Защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="27aa1-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="27aa1-105">Политика Windows Endpoint Protection дает возможность создавать в Intune дополнительные параметры для функций Защитника Windows и применять их к наборам устройств.</span><span class="sxs-lookup"><span data-stu-id="27aa1-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="27aa1-106">Дополнительные сведения о запуске действий Защитника Windows см. в статье [Настройка и запуск проверки антивирусной программы в Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="27aa1-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>
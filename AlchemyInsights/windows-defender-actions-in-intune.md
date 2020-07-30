---
title: Действия Защитника Windows в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434628"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="bfeb3-102">Действия Защитника Windows в Intune</span><span class="sxs-lookup"><span data-stu-id="bfeb3-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="bfeb3-103">Можно использовать Intune, чтобы запускать проверку по запросу и обновлять сигнатуры вирусов в Защитнике Windows на отдельных устройствах.</span><span class="sxs-lookup"><span data-stu-id="bfeb3-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="bfeb3-104">После успешного запуска удаленного действия это действие записывается в журнале событий Защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="bfeb3-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="bfeb3-105">Политика Windows Endpoint Protection дает возможность создавать в Intune дополнительные параметры для функций Защитника Windows и применять их к наборам устройств.</span><span class="sxs-lookup"><span data-stu-id="bfeb3-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="bfeb3-106">Дополнительные сведения о запуске действий Защитника Windows см. в статье [Настройка и запуск проверки антивирусной программы в Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="bfeb3-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>
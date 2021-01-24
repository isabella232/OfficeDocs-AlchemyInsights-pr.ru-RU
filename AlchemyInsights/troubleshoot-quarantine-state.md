---
title: Устранение неполадок, связанных с состоянием карантина
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935399"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="76f69-102">Устранение неполадок, связанных с состоянием карантина</span><span class="sxs-lookup"><span data-stu-id="76f69-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="76f69-103">Служба подготовки Azure Active Directory (AD) следит за состоянием вашей конфигурации.</span><span class="sxs-lookup"><span data-stu-id="76f69-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="76f69-104">Она также помещает неработоспособные приложения в состояние **карантина**.</span><span class="sxs-lookup"><span data-stu-id="76f69-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="76f69-105">Если большинство вызовов или все вызовы, относящиеся к конечной системе, постоянно завершаются сбоем, задание подготовки помечается как находящееся **на карантине**.</span><span class="sxs-lookup"><span data-stu-id="76f69-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="76f69-106">Примером сбоя является **ошибка, полученная из-за недопустимых учетных данных администратора**.</span><span class="sxs-lookup"><span data-stu-id="76f69-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="76f69-107">Дополнительные сведения см. в статье [Подготовка приложения в состоянии карантина](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span><span class="sxs-lookup"><span data-stu-id="76f69-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="76f69-108">Чтобы устранить проблемы с облачной синхронизацией, см. статью [Проблемы подготовки на карантине](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span><span class="sxs-lookup"><span data-stu-id="76f69-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 

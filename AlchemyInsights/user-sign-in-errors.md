---
title: Ошибки пользователя при входе
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886891"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="1bc03-102">Ошибки пользователя при входе</span><span class="sxs-lookup"><span data-stu-id="1bc03-102">User sign-in errors</span></span>

<span data-ttu-id="1bc03-103">**Устранение проблем с диагностикой входа**</span><span class="sxs-lookup"><span data-stu-id="1bc03-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="1bc03-104">Чтобы найти причину проблемы или диагностировать ошибки, связанные со входом пользователя, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1bc03-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="1bc03-105">Запустите [Диагностику входа](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="1bc03-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="1bc03-106">Найдите событие, которое нужно проанализировать, указав сведения о пользователе, приложении, времени входа, идентификаторе запроса или корреляции.</span><span class="sxs-lookup"><span data-stu-id="1bc03-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="1bc03-107">Ознакомьтесь с результатами диагностики, отображающими подробные сведения о том, что произошло и какие действия нужно предпринять, чтобы внести изменения.</span><span class="sxs-lookup"><span data-stu-id="1bc03-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="1bc03-108">**Ищете информацию о кодах ошибок AADSTS, которые возвращаются из службы маркеров безопасности (STS) Azure Active Directory (Azure AD)?**</span><span class="sxs-lookup"><span data-stu-id="1bc03-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="1bc03-109">В [этой статье](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) приводятся описание ошибок AADSTS, способы их устранения и несколько рекомендаций по устранению неполадок.</span><span class="sxs-lookup"><span data-stu-id="1bc03-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>
---
title: Метки конфиденциальности не отображаются
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048665"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="bc445-102">Метки конфиденциальности не отображаются</span><span class="sxs-lookup"><span data-stu-id="bc445-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="bc445-103">Метки конфиденциальности позволяют классифицировать и защищать конфиденциальное содержимое.</span><span class="sxs-lookup"><span data-stu-id="bc445-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="bc445-104">Они могут быть созданы в центре соответствия требованиям Microsoft 365, центре безопасности 365 Майкрософт или Office 365 центр соответствия требованиям & безопасности в разделе классификация > меток конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bc445-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="bc445-105">Чтобы узнать больше об этой функции, просмотрите раздел [Обзор меток конфиденциальности](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="bc445-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="bc445-106">Если вы настроили метки конфиденциальности, но они не отображаются в приложениях Office, проверьте следующее:</span><span class="sxs-lookup"><span data-stu-id="bc445-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="bc445-107">Убедитесь, что метка конфиденциальности была [опубликована](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) для нужных пользователей и групп.</span><span class="sxs-lookup"><span data-stu-id="bc445-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="bc445-108">Убедитесь, что пользователь использует приложение, которое поддерживает метки чувствительности — просмотрите [метки конфиденциальности в документе](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="bc445-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="bc445-109">Если вы переносите [метки Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), учитывайте вопросы, приведенные в [этой статье](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="bc445-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="bc445-110">Поддержка защиты от потери данных (DLP): в настоящее время в качестве условия в политиках защиты от потери данных можно использовать только метки хранения.</span><span class="sxs-lookup"><span data-stu-id="bc445-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="bc445-111">Поддержка меток конфиденциальности в политике DLP пока недоступна, но мы работаем над этим.</span><span class="sxs-lookup"><span data-stu-id="bc445-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="bc445-112">Если для метки конфиденциальности включено шифрование, вы можете выбрать один из следующих вариантов:</span><span class="sxs-lookup"><span data-stu-id="bc445-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="bc445-113">Назначение разрешений сразу</span><span class="sxs-lookup"><span data-stu-id="bc445-113">Assign permissions now</span></span>
    - <span data-ttu-id="bc445-114">Предоставление пользователям возможности назначать разрешения</span><span class="sxs-lookup"><span data-stu-id="bc445-114">Let users assign permissions</span></span>


<span data-ttu-id="bc445-115">Дополнительные сведения о возможных проблемах приведены в статье [Известные проблемы с метками чувствительности](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="bc445-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>
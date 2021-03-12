---
title: DLP не работает так, как ожидалось
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707823"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="3402d-102">DLP не работает так, как ожидалось</span><span class="sxs-lookup"><span data-stu-id="3402d-102">DLP not working as expected</span></span>

<span data-ttu-id="3402d-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="3402d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="3402d-104">**Настройка DLP**</span><span class="sxs-lookup"><span data-stu-id="3402d-104">**Setting up DLP**</span></span>

<span data-ttu-id="3402d-105">У вас возникли проблемы с предотвращением потери данных **(DLP)** в Office 365 не работает, как ожидалось?</span><span class="sxs-lookup"><span data-stu-id="3402d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="3402d-106">Если это так, убедитесь, что политика **DLP** настроена правильно и ваши данные содержат то, что ищет политика **DLP** при оценке.</span><span class="sxs-lookup"><span data-stu-id="3402d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="3402d-107">Политики DLP позволяют выявлять и защищать конфиденциальные сведения в организации.</span><span class="sxs-lookup"><span data-stu-id="3402d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="3402d-108">Чтобы настроить политики DLP, используйте сведения [здесь.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="3402d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="3402d-109">**Какие политики DLP**</span><span class="sxs-lookup"><span data-stu-id="3402d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="3402d-110">При использовании **встроенных** типов конфиденциальной информации в центрах безопасности и соответствия требованиям политики DLP при обнаружении этих конфиденциальных типов и элементов будут искать определенные шаблоны и элементы.</span><span class="sxs-lookup"><span data-stu-id="3402d-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="3402d-111">**Встроенные типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="3402d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="3402d-112">Сведения о встроенных конфиденциальных типах и о том, что ищет политика DLP при обнаружении типа Sensitive, [см.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)в этой таблице.</span><span class="sxs-lookup"><span data-stu-id="3402d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="3402d-113">**Настраиваемые типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="3402d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="3402d-114">Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого конфиденциального типа: Создание настраиваемого типа [конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="3402d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="3402d-115">**Тестирование политики DLP**</span><span class="sxs-lookup"><span data-stu-id="3402d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="3402d-116">Чтобы протестировать данные с помощью встроенного или настраиваемого типа конфиденциальной информации, используйте параметр **Test type** в **типах Classifications**  >  **Sensitive info types.**</span><span class="sxs-lookup"><span data-stu-id="3402d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="3402d-117">Дополнительные сведения см. в [специальном тесте типов конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="3402d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="3402d-118">**Отчеты**</span><span class="sxs-lookup"><span data-stu-id="3402d-118">**Reports**</span></span>
  
- <span data-ttu-id="3402d-119">Получите конфиденциальные сведения о данных с [помощью отчетов DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="3402d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="3402d-120">Дополнительные сведения о событии см. в [отчете об инциденте.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="3402d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>

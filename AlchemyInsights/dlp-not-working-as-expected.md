---
title: Защита от потери данных не работает должным образом
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977451"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f6c1d-102">Защита от потери данных не работает должным образом</span><span class="sxs-lookup"><span data-stu-id="f6c1d-102">DLP not working as expected</span></span>

<span data-ttu-id="f6c1d-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f6c1d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="f6c1d-104">**Настройка защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-104">**Setting up DLP**</span></span>

<span data-ttu-id="f6c1d-105">Проблемы с **предотвращением потери данных (DLP)** в Office 365 не работают должным образом?</span><span class="sxs-lookup"><span data-stu-id="f6c1d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f6c1d-106">Если это так, убедитесь, что **Политика защиты от потери** данных настроена правильно, а данные содержат сведения о том, какую **политику DLP** ищет при оценке.</span><span class="sxs-lookup"><span data-stu-id="f6c1d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="f6c1d-107">Политики DLP позволяют определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="f6c1d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f6c1d-108">Чтобы настроить политики защиты от потери данных, используйте [здесь](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="f6c1d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f6c1d-109">**Поиск в политиках защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f6c1d-110">При использовании **встроенных типов конфиденциальной информации** в центре безопасности и соответствия требованиям Office 365 политики DLP ищут конкретные закономерности и элементы при обнаружении этих конфиденциальных типов.</span><span class="sxs-lookup"><span data-stu-id="f6c1d-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f6c1d-111">**Встроенные типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f6c1d-112">Для получения сведений о встроенных конфиденциальных типах и действиях, выполняемых политикой DLP при определении конфиденциального типа, ознакомьтесь со статьей: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="f6c1d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="f6c1d-113">**Настраиваемые типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f6c1d-114">Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого типа конфиденциальной [информации: Создание настраиваемого типа конфиденциальной информации](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f6c1d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f6c1d-115">**Проверка политики DLP**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="f6c1d-116">Чтобы протестировать данные со встроенным или настраиваемым типом конфиденциальной информации, используйте параметр **тип теста** в разделе **классификация** > **типов конфиденциальной**информации.</span><span class="sxs-lookup"><span data-stu-id="f6c1d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f6c1d-117">Дополнительные [сведения см.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="f6c1d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f6c1d-118">**Отчеты**</span><span class="sxs-lookup"><span data-stu-id="f6c1d-118">**Reports**</span></span>
  
- <span data-ttu-id="f6c1d-119">Получение конфиденциальных данных с помощью [отчетов о](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) защите от потери данных.</span><span class="sxs-lookup"><span data-stu-id="f6c1d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f6c1d-120">Просмотр определенных сведений о событии с [отчетом об инциденте](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="f6c1d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>

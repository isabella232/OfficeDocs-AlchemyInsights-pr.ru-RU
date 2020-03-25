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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932635"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="53d51-102">Защита от потери данных не работает должным образом</span><span class="sxs-lookup"><span data-stu-id="53d51-102">DLP not working as expected</span></span>

<span data-ttu-id="53d51-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="53d51-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="53d51-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="53d51-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="53d51-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="53d51-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="53d51-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="53d51-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="53d51-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="53d51-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="53d51-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="53d51-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="53d51-109">**Настройка защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="53d51-109">**Setting up DLP**</span></span>

<span data-ttu-id="53d51-110">Проблемы с **предотвращением потери данных (DLP)** в Office 365 не работают должным образом?</span><span class="sxs-lookup"><span data-stu-id="53d51-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="53d51-111">Если это так, убедитесь, что **Политика защиты от потери** данных настроена правильно, а данные содержат сведения о том, какую **политику DLP** ищет при оценке.</span><span class="sxs-lookup"><span data-stu-id="53d51-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="53d51-112">Политики DLP позволяют определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="53d51-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="53d51-113">Чтобы настроить политики защиты от потери данных, используйте [здесь](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="53d51-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="53d51-114">**Поиск в политиках защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="53d51-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="53d51-115">При использовании **встроенных типов конфиденциальной информации** в центре безопасности и соответствия требованиям Office 365 политики DLP ищут конкретные закономерности и элементы при обнаружении этих конфиденциальных типов.</span><span class="sxs-lookup"><span data-stu-id="53d51-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="53d51-116">**Встроенные типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="53d51-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="53d51-117">Для получения сведений о встроенных конфиденциальных типах и действиях, выполняемых политикой DLP при определении конфиденциального типа, ознакомьтесь со статьей: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="53d51-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="53d51-118">**Настраиваемые типы конфиденциальной информации**</span><span class="sxs-lookup"><span data-stu-id="53d51-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="53d51-119">Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого типа конфиденциальной [информации: Создание настраиваемого типа конфиденциальной информации](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="53d51-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="53d51-120">**Проверка политики DLP**</span><span class="sxs-lookup"><span data-stu-id="53d51-120">**Test a DLP policy**</span></span>

<span data-ttu-id="53d51-121">Чтобы протестировать данные со встроенным или настраиваемым типом конфиденциальной информации, используйте параметр **тип теста** в разделе **классификация** > **типов конфиденциальной**информации.</span><span class="sxs-lookup"><span data-stu-id="53d51-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="53d51-122">Дополнительные [сведения см.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="53d51-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="53d51-123">**Отчеты**</span><span class="sxs-lookup"><span data-stu-id="53d51-123">**Reports**</span></span>
  
- <span data-ttu-id="53d51-124">Получение конфиденциальных данных с помощью [отчетов о](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) защите от потери данных.</span><span class="sxs-lookup"><span data-stu-id="53d51-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="53d51-125">Просмотр определенных сведений о событии с [отчетом об инциденте](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="53d51-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>

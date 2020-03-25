---
title: Для защиты от потери данных может потребоваться настраиваемый тип
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932671"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d9f8c-102">Для защиты от потери данных может потребоваться настраиваемый тип</span><span class="sxs-lookup"><span data-stu-id="d9f8c-102">DLP might need a custom type</span></span>

<span data-ttu-id="d9f8c-103">**Важно!** многие клиенты SharePoint Online и OneDrive работают с критическими бизнес-приложениями для службы, которая работает в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d9f8c-104">В их число входят перенос контента, защита от потери данных и решения для резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d9f8c-105">В это беспрецедентное время мы работаем над тем, чтобы службы SharePoint Online и OneDrive оставались высокодоступными и надежными для пользователей, которые зависят от них более, чем когда-либо, в связи с удаленной работой.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d9f8c-106">Для этого мы установили более жесткие ограничения регулирования для фоновых приложений (миграция, защита от потери данных и решения для резервного копирования) в рабочие дни в дневное время.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d9f8c-107">Ожидается, что теперь пропускная способность этих приложений будет очень ограничена.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d9f8c-108">Однако в вечернее время и на выходных (для данного региона) служба будет готова обработать значительно больший объем запросов от фоновых приложений.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d9f8c-109">**Для защиты от потери данных может потребоваться настраиваемый тип данных**</span><span class="sxs-lookup"><span data-stu-id="d9f8c-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d9f8c-110">С помощью политики защиты от потери данных (DLP) вы можете определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d9f8c-111">В некоторых случаях может потребоваться создать собственный **Настраиваемый** тип конфиденциальной информации для защиты данных Организации.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d9f8c-112">Например, вашей организации может потребоваться определить и защитить идентификаторы сотрудников или другие данные в определенном формате, характерном для вашей организации. Если это так, ознакомьтесь со следующими статьями, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d9f8c-113">**Настройка встроенных типов конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="d9f8c-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d9f8c-114">Если встроенный тип конфиденциальной информации соответствует вашим потребностям с помощью всего нескольких настроек, можно [настроить встроенный тип конфиденциальной информации](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d9f8c-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d9f8c-115">Например, можно добавлять или удалять ключевые слова, а также добавлять или удалять поддерживающие их доказательства, такие как дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d9f8c-116">**Создание пользовательского типа конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="d9f8c-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d9f8c-117">Но если вам нужно полностью определить и защитить конфиденциальную информацию, вы можете [создать настраиваемый тип конфиденциальной информации](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) в пользовательском интерфейсе центра безопасности & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d9f8c-118">**Создание пользовательского типа конфиденциальной информации в PowerShell Центра безопасности и соответствия требованиям**</span><span class="sxs-lookup"><span data-stu-id="d9f8c-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d9f8c-119">Наконец, если пользовательский интерфейс не предоставляет все необходимые параметры, можно [создать настраиваемый тип конфиденциальной информации в оболочке безопасности & центра соответствия требованиям](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d9f8c-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d9f8c-120">Начиная с XML-файла, можно использовать все доступные параметры.</span><span class="sxs-lookup"><span data-stu-id="d9f8c-120">By starting with an XML file, you can use every option available.</span></span>

---
title: Для защиты от потери данных может потребоваться настраиваемый тип
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712197"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2e882-102">Для защиты от потери данных может потребоваться настраиваемый тип</span><span class="sxs-lookup"><span data-stu-id="2e882-102">DLP might need a custom type</span></span>

<span data-ttu-id="2e882-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2e882-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2e882-104">**Для защиты от потери данных может потребоваться настраиваемый тип данных**</span><span class="sxs-lookup"><span data-stu-id="2e882-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2e882-105">С помощью политики защиты от потери данных (DLP) вы можете определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="2e882-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2e882-106">В некоторых случаях может потребоваться создать собственный **Настраиваемый** тип конфиденциальной информации для защиты данных Организации.</span><span class="sxs-lookup"><span data-stu-id="2e882-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2e882-107">Например, вашей организации может потребоваться определить и защитить идентификаторы сотрудников или другие данные в определенном формате, характерном для вашей организации. Если это так, ознакомьтесь со следующими статьями, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="2e882-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2e882-108">**Настройка встроенных типов конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="2e882-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2e882-109">Если встроенный тип конфиденциальной информации соответствует вашим потребностям с помощью всего нескольких настроек, можно [настроить встроенный тип конфиденциальной информации](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2e882-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2e882-110">Например, можно добавлять или удалять ключевые слова, а также добавлять или удалять поддерживающие их доказательства, такие как дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="2e882-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2e882-111">**Создание пользовательского типа конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="2e882-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2e882-112">Но если вам нужно полностью определить и защитить конфиденциальную информацию, вы можете [создать настраиваемый тип конфиденциальной информации](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) в пользовательском интерфейсе центра безопасности & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2e882-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2e882-113">**Создание пользовательского типа конфиденциальной информации в PowerShell Центра безопасности и соответствия требованиям**</span><span class="sxs-lookup"><span data-stu-id="2e882-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2e882-114">Наконец, если пользовательский интерфейс не предоставляет все необходимые параметры, можно [создать настраиваемый тип конфиденциальной информации в оболочке безопасности & центра соответствия требованиям](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2e882-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2e882-115">Начиная с XML-файла, можно использовать все доступные параметры.</span><span class="sxs-lookup"><span data-stu-id="2e882-115">By starting with an XML file, you can use every option available.</span></span>

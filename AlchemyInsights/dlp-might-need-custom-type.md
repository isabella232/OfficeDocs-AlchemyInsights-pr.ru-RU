---
title: Для защиты от потери данных может потребоваться настраиваемый тип
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2019
ms.locfileid: "31872468"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6d95c-102">Для защиты от потери данных может потребоваться настраиваемый тип</span><span class="sxs-lookup"><span data-stu-id="6d95c-102">DLP might need a custom type</span></span>

<span data-ttu-id="6d95c-103">С помощью политики защиты от потери данных (DLP) вы можете определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="6d95c-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6d95c-104">В некоторых случаях может потребоваться создать собственный **Настраиваемый** тип конфиденциальной информации для защиты данных Организации.</span><span class="sxs-lookup"><span data-stu-id="6d95c-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6d95c-105">Например, вашей организации может потребоваться определить и защитить идентификаторы сотрудников или другие данные в определенном формате, характерном для вашей организации. Если это так, ознакомьтесь со следующими статьями, чтобы получить дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="6d95c-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="6d95c-106">**Настройка встроенных типов конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="6d95c-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6d95c-107">Если встроенный тип конфиденциальной информации соответствует вашим потребностям с помощью всего нескольких настроек, можно [настроить встроенный тип конфиденциальной информации](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6d95c-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6d95c-108">Например, можно добавлять или удалять ключевые слова, а также добавлять или удалять поддерживающие их доказательства, такие как дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="6d95c-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6d95c-109">**Создание пользовательского типа конфиденциальных данных**</span><span class="sxs-lookup"><span data-stu-id="6d95c-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6d95c-110">Но если вам нужно полностью определить и защитить конфиденциальную информацию, вы можете [создать настраиваемый тип конфиденциальной информации](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) в пользовательском интерфейсе центра соответствия требованиям безопасности _амп_.</span><span class="sxs-lookup"><span data-stu-id="6d95c-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="6d95c-111">**Создание пользовательского типа конфиденциальной информации в PowerShell центра соответствия требованиям безопасности _Амп_**</span><span class="sxs-lookup"><span data-stu-id="6d95c-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6d95c-112">Наконец, если пользовательский интерфейс не предоставляет все необходимые параметры, можно [создать настраиваемый тип конфиденциальной информации в PowerShell Security _Амп_ Security Center](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6d95c-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6d95c-113">Начиная с XML-файла, можно использовать все доступные параметры.</span><span class="sxs-lookup"><span data-stu-id="6d95c-113">By starting with an XML file, you can use every option available.</span></span>

    

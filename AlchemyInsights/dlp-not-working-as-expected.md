---
title: Защита от потери данных не работает должным образом
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 6d8e3e540494e99e42f04080681f46324f2936bd
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2019
ms.locfileid: "31869572"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="92d75-102">Защита от потери данных не работает должным образом</span><span class="sxs-lookup"><span data-stu-id="92d75-102">DLP not working as expected</span></span>


<span data-ttu-id="92d75-103">Проблемы с **предотвращением потери данных (DLP)** в Office 365 не работают должным образом?</span><span class="sxs-lookup"><span data-stu-id="92d75-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="92d75-104">Если это так, убедитесь, что **Политика защиты от потери** данных настроена правильно, а данные содержат сведения о том, какую **политику DLP** ищет при оценке.</span><span class="sxs-lookup"><span data-stu-id="92d75-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="92d75-105">**Настройка защиты от потери данных:**</span><span class="sxs-lookup"><span data-stu-id="92d75-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="92d75-106">Политики DLP позволяют определять и защищать конфиденциальные данные в Организации.</span><span class="sxs-lookup"><span data-stu-id="92d75-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="92d75-107">Чтобы настроить политики защиты от потери данных, используйте [здесь](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="92d75-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="92d75-108">**Поиск политик защиты от потери данных:**</span><span class="sxs-lookup"><span data-stu-id="92d75-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="92d75-109">При использовании **встроенных типов конфиденциальной информации** в центре безопасности и соответствия требованиям Office 365 политики DLP ищут конкретные закономерности и элементы при обнаружении этих конфиденциальных типов.</span><span class="sxs-lookup"><span data-stu-id="92d75-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="92d75-110">**Встроенные типы конфиденциальной информации:**</span><span class="sxs-lookup"><span data-stu-id="92d75-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="92d75-111">Для получения сведений о встроенных конфиденциальных типах и действиях, выполняемых политикой DLP при определении конфиденциального типа, ознакомьтесь со статьей: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="92d75-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="92d75-112">**Настраиваемые типы конфиденциальной информации:**</span><span class="sxs-lookup"><span data-stu-id="92d75-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="92d75-113">Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого типа конфиденциальной [информации: Создание настраиваемого типа конфиденциальной информации](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="92d75-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="92d75-114">**Определяется**</span><span class="sxs-lookup"><span data-stu-id="92d75-114">**Reports:**</span></span>
  
- <span data-ttu-id="92d75-115">Получение конфиденциальных данных с помощью [отчетов о](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports) защите от потери данных.</span><span class="sxs-lookup"><span data-stu-id="92d75-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="92d75-116">Просмотр определенных сведений о событии с отчетом об [инциденте](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="92d75-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    


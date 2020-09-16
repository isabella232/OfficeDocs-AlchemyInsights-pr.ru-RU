---
title: Списание службы Azure Rights Management (RMS)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5070"
- "9002278"
ms.openlocfilehash: 6bacfd0e383c1a7c02b50e60f9626a733ee68cbc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745800"
---
# <a name="decommission-azure-rights-management-service-rms"></a><span data-ttu-id="71ad3-102">Списание службы Azure Rights Management (RMS)</span><span class="sxs-lookup"><span data-stu-id="71ad3-102">Decommission Azure Rights Management Service (RMS)</span></span>

<span data-ttu-id="71ad3-103">Прежде чем отключать службу Azure Rights Management, убедитесь в том, что у вас есть копия ключа клиента Azure Information Protection и подходящий доверенный домен публикации (TPD).</span><span class="sxs-lookup"><span data-stu-id="71ad3-103">Make sure that you have a copy of your Azure Information Protection tenant key and a suitable trusted publishing domain (TPD) before you deactivate the Azure Rights Management service.</span></span>

<span data-ttu-id="71ad3-104">Дополнительные ресурсы о списании службы и отключении защиты в Azure Information Protection см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="71ad3-104">For additional resources about decommissioning and deactivating protection for Azure Information Protection, see:</span></span>

- [<span data-ttu-id="71ad3-105">Руководство: настройка параметров политики Azure Information Protection и создание новой метки</span><span class="sxs-lookup"><span data-stu-id="71ad3-105">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="71ad3-106">Что такое Azure Information Protection?</span><span class="sxs-lookup"><span data-stu-id="71ad3-106">What is Azure Information Protection?</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="71ad3-107">Пошаговые инструкции для распространенных сценариев, в которых используется Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="71ad3-107">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
    
- [<span data-ttu-id="71ad3-108">Способ переноса меток Azure Information Protection в платформу унифицированных меток конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="71ad3-108">How to migrate Azure Information Protection labels to unified sensitivity labels</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)  
    
- [<span data-ttu-id="71ad3-109">Ценообразование в Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="71ad3-109">Azure Information Protection pricing</span></span>](https://azure.microsoft.com/pricing/details/information-protection)  
    
- [<span data-ttu-id="71ad3-110">Требования Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="71ad3-110">Azure Information Protection requirements</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
    
- [<span data-ttu-id="71ad3-111">Активация службы защиты Rights Management на портале Azure</span><span class="sxs-lookup"><span data-stu-id="71ad3-111">How to activate the Rights Management protection service from the Azure portal</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-use/activate-azure)
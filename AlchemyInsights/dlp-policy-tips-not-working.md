---
title: Советы политики защиты от потери данных не работают
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679598"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="ae297-102">Проблемы с подсказкой политики DLP</span><span class="sxs-lookup"><span data-stu-id="ae297-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="ae297-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ae297-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ae297-104">**Советы по политике защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="ae297-104">**DLP policy tips**</span></span>

<span data-ttu-id="ae297-105">При использовании **политик защиты от потери**данных пользователи могут получать уведомления о нарушении политики с помощью **подсказок политики**.</span><span class="sxs-lookup"><span data-stu-id="ae297-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="ae297-106">Администраторы могут настроить подсказки политики для отображения при тестировании политики защиты от потери данных или когда политика находится в режиме полной принудительной защиты.</span><span class="sxs-lookup"><span data-stu-id="ae297-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="ae297-107">Чтобы настроить подсказки политики для политики защиты от потери данных в центре безопасности и соответствия требованиям в режиме полного применения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ae297-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="ae297-108">Убедитесь, что подсказка политики **включена** для правила DLP, выполнив действия, описанные в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="ae297-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="ae297-109">Убедитесь, что **контент соответствует** тому, что **требуется** для запуска правила, описанного в этой [статье.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="ae297-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="ae297-110">Подсказка политики отображается как в OWA, так и в Outlook.</span><span class="sxs-lookup"><span data-stu-id="ae297-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="ae297-111">Однако при использовании **Outlook 2013 или более поздней версии**подсказки политики отображаются только при определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="ae297-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="ae297-112">Эти условия перечислены ниже: [Поддерживаемые условия для Outlook 2013 или более поздней версии для отображения подсказок политики](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="ae297-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="ae297-113">Дополнительные сведения о подсказках политики DLP: [show policy подсказки для политик защиты от потери](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips) данных</span><span class="sxs-lookup"><span data-stu-id="ae297-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  
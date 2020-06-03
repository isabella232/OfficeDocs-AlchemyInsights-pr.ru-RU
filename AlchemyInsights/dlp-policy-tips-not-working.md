---
title: Советы политики защиты от потери данных не работают
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 9369878b62a5abe79bd215487bea6cabb0e80f06
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507455"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="5a4fc-102">Проблемы с подсказкой политики DLP</span><span class="sxs-lookup"><span data-stu-id="5a4fc-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="5a4fc-103">**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="5a4fc-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5a4fc-104">**Советы по политике защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="5a4fc-104">**DLP policy tips**</span></span>

<span data-ttu-id="5a4fc-105">При использовании **политик защиты от потери**данных пользователи могут получать уведомления о нарушении политики с помощью **подсказок политики**.</span><span class="sxs-lookup"><span data-stu-id="5a4fc-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="5a4fc-106">Администраторы могут настроить подсказки политики для отображения при тестировании политики защиты от потери данных или когда политика находится в режиме полной принудительной защиты.</span><span class="sxs-lookup"><span data-stu-id="5a4fc-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="5a4fc-107">Чтобы настроить подсказки политики для политики защиты от потери данных в центре безопасности и соответствия требованиям в режиме полного применения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="5a4fc-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="5a4fc-108">Убедитесь, что подсказка политики **включена** для правила DLP, выполнив действия, описанные в [этой статье](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="5a4fc-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="5a4fc-109">Убедитесь, что **контент соответствует** тому, что **требуется** для запуска правила, описанного в этой [статье.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5a4fc-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="5a4fc-110">Подсказка политики отображается как в OWA, так и в Outlook.</span><span class="sxs-lookup"><span data-stu-id="5a4fc-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="5a4fc-111">Однако при использовании **Outlook 2013 или более поздней версии**подсказки политики отображаются только при определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="5a4fc-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="5a4fc-112">Эти условия перечислены ниже: [Поддерживаемые условия для Outlook 2013 или более поздней версии для отображения подсказок политики](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="5a4fc-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="5a4fc-113">Дополнительные сведения о подсказках политики DLP: [show policy подсказки для политик защиты от потери](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips) данных</span><span class="sxs-lookup"><span data-stu-id="5a4fc-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  
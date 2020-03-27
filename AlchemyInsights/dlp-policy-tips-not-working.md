---
title: Советы политики защиты от потери данных не работают
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 6375fa8077529f36ae95d6632ad4d2db5625dc29
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977247"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="cb00f-102">Проблемы с подсказкой политики DLP</span><span class="sxs-lookup"><span data-stu-id="cb00f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="cb00f-103">**Важно!** в это незначительное время мы предоставим вам рекомендации по включению служб SharePoint Online и OneDrive, чтобы получить дополнительные сведения о [временных функциях SharePoint](https://aka.ms/ODSPAdjustments) Online.</span><span class="sxs-lookup"><span data-stu-id="cb00f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cb00f-104">**Советы по политике защиты от потери данных**</span><span class="sxs-lookup"><span data-stu-id="cb00f-104">**DLP policy tips**</span></span>

<span data-ttu-id="cb00f-105">При использовании **политик защиты от потери**данных пользователи могут получать уведомления о нарушении политики с помощью **подсказок политики**.</span><span class="sxs-lookup"><span data-stu-id="cb00f-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="cb00f-106">Администраторы могут настроить подсказки политики для отображения при тестировании политики защиты от потери данных или когда политика находится в режиме полной принудительной защиты.</span><span class="sxs-lookup"><span data-stu-id="cb00f-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="cb00f-107">Чтобы настроить подсказки политики для политики защиты от потери данных в центре безопасности и соответствия требованиям в режиме полного применения, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="cb00f-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="cb00f-108">Убедитесь, что подсказка политики **включена** для правила DLP, выполнив действия, описанные в [этой статье](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="cb00f-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="cb00f-109">Убедитесь, что **контент соответствует** тому, что **требуется** для запуска правила, описанного в этой [статье.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cb00f-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="cb00f-110">Подсказка политики отображается как в OWA, так и в Outlook.</span><span class="sxs-lookup"><span data-stu-id="cb00f-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="cb00f-111">Однако при использовании **Outlook 2013 или более поздней версии**подсказки политики отображаются только при определенных условиях.</span><span class="sxs-lookup"><span data-stu-id="cb00f-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="cb00f-112">Эти условия перечислены ниже: [Поддерживаемые условия для Outlook 2013 или более поздней версии для отображения подсказок политики](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="cb00f-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="cb00f-113">Дополнительные сведения о подсказках политики DLP: [show policy подсказки для политик защиты от потери](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) данных</span><span class="sxs-lookup"><span data-stu-id="cb00f-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  
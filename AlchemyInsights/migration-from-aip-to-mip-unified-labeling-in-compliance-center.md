---
title: Миграция с AIP на MIP/унифицированные метки в Центре соответствия требованиям
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236572"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="6db87-102">Миграция с AIP на MIP/унифицированные метки в Центре соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6db87-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="6db87-103">Чтобы перейти с меток AIP на унифицированные метки в Центре безопасности и соответствия требованиям, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="6db87-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="6db87-104">**Активация защиты из портала Azure**</span><span class="sxs-lookup"><span data-stu-id="6db87-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="6db87-105">Если вы этого еще не сделали, откройте новое окно браузера и [войдите на портал Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="6db87-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="6db87-106">Перейдите к колонке **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="6db87-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="6db87-107">Например, в главном меню щелкните **Все службы** и начните вводить **Information** в поле фильтра.</span><span class="sxs-lookup"><span data-stu-id="6db87-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="6db87-108">Выберите **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="6db87-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="6db87-109">Если вы ранее не обращались к колонке Azure Information Protection, ознакомьтесь с однократными [дополнительными действиями](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) по ее добавлению на портал.</span><span class="sxs-lookup"><span data-stu-id="6db87-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="6db87-110">Чтобы открыть колонку Azure Information Protection, у вас должен быть [план Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)или план Office 365, включающий управление правами.</span><span class="sxs-lookup"><span data-stu-id="6db87-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="6db87-111">Если у вас есть одна из этих подписок, но появляется сообщение об отсутствии надлежащей подписки, [обратитесь в службу поддержки Майкрософт](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или используйте стандартные каналы поддержки.</span><span class="sxs-lookup"><span data-stu-id="6db87-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="6db87-112">Найдите параметры меню **Управление** и выберите **Активация защиты**.</span><span class="sxs-lookup"><span data-stu-id="6db87-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="6db87-113">Щелкните **Активировать** и подтвердите действие.</span><span class="sxs-lookup"><span data-stu-id="6db87-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="6db87-114">После завершения активации на информационной панели отобразится сообщение **Активация успешно завершена**.</span><span class="sxs-lookup"><span data-stu-id="6db87-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="6db87-115">**Перенос меток Azure Information Protection в Центр безопасности и соответствия требованиям Office 365**</span><span class="sxs-lookup"><span data-stu-id="6db87-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="6db87-116">Войдите в качестве пользователя с разрешениями глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="6db87-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="6db87-117">Перейдите к колонке **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="6db87-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="6db87-118">В меню **Управление** выберите параметр **Унифицированные метки**.</span><span class="sxs-lookup"><span data-stu-id="6db87-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="6db87-119">В колонке **Azure Information Protection — Унифицированные метки** щелкните **Активировать** и следуйте инструкциям в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6db87-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="6db87-120">**Примечание**. Проверьте наличие соответствующих разрешений перед активацией миграции в Центр безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="6db87-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="6db87-121">Дополнительные сведения см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="6db87-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="6db87-122">Необходимо ли быть глобальным администратором для настройки Azure Information Protection? Или выполнение этой задачи можно делегировать другим администраторам?</span><span class="sxs-lookup"><span data-stu-id="6db87-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. <span data-ttu-id="6db87-123">[Важные сведения об административных ролях после миграции в Центр безопасности и соответствия требованиям](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles).</span><span class="sxs-lookup"><span data-stu-id="6db87-123">[Important information about administrative roles after migrating to Security & Compliance Center.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)</span></span>

<span data-ttu-id="6db87-124">Дополнительные сведения о миграции с AIP на унифицированные метки в Центре безопасности и соответствия требованиям см. в статье [Перенос меток](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="6db87-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>

---
title: Невозможно войти в Команды из-за ошибки autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932033"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="3385e-102">Невозможно войти в Команды из-за ошибки autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="3385e-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="3385e-103">Если в качестве аутентификации O365 включен бесшовный SSO, возможно, необходимо добавить URL-адрес autologon.microsoftazuread-sso.com в сайты интрасети.</span><span class="sxs-lookup"><span data-stu-id="3385e-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="3385e-104">Если он ранее был добавлен в доверенные сайты и используется бесшовная служба единого входа, его следует удалить из доверенных сайтов.</span><span class="sxs-lookup"><span data-stu-id="3385e-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="3385e-105">Пожалуйста, ознакомьтесь с [контрольным списком проблем с единой системой единого входа](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="3385e-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="3385e-106">Выполните следующие действия, чтобы добавить URL-адрес в список сайтов интрасети:</span><span class="sxs-lookup"><span data-stu-id="3385e-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="3385e-107">Откройте Internet Explorer, нажав кнопку **Пуск**.</span><span class="sxs-lookup"><span data-stu-id="3385e-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="3385e-108">В поле поиска введите Internet Explorer, а затем в списке результатов щелкните **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="3385e-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="3385e-109">Нажмите **Инструменты**, а затем нажмите **Свойства обозревателя**.</span><span class="sxs-lookup"><span data-stu-id="3385e-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="3385e-110">Щелкните вкладку **Безопасность**.</span><span class="sxs-lookup"><span data-stu-id="3385e-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="3385e-111">Теперь нажмите на **сайты локальной интрасети**, затем нажмите кнопку **сайтов** и затем кнопку **Дополнительно**.</span><span class="sxs-lookup"><span data-stu-id="3385e-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="3385e-112">Введите URL-адрес веб-сайта и нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="3385e-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="3385e-113">Когда вы закончите, нажмите **Закрыть**.</span><span class="sxs-lookup"><span data-stu-id="3385e-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="3385e-114">Для получения дополнительной информации см. [Документация по развертыванию бесшовного единого входа для O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (включает процесс на основе политик для добавления URL-адреса на сайты интрасети на шаге 3).</span><span class="sxs-lookup"><span data-stu-id="3385e-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>

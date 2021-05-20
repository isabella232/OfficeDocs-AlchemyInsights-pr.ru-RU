---
title: Симулятор атаки 2681 в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545739"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="0aa87-102">Симулятор атаки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0aa87-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="0aa87-103">Отсутствует симулятор атак?</span><span class="sxs-lookup"><span data-stu-id="0aa87-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="0aa87-104">Симулятор атак требует **microsoft Defender для Office 365 плана 2** или Office 365 корпоративный **E5.**</span><span class="sxs-lookup"><span data-stu-id="0aa87-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="0aa87-105">Симулятор атак **не входит** в Microsoft Defender для Office 365 плана 1, Office 365 корпоративный E3 или Приложения Microsoft 365 для бизнеса подписки.</span><span class="sxs-lookup"><span data-stu-id="0aa87-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="0aa87-106">Учетная запись, используемая для запуска имитации атак, требует разрешений глобального администратора или администратора безопасности и многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="0aa87-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="0aa87-107">Дополнительные сведения о требованиях к симулятору атак см. [в этом разделе.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="0aa87-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="0aa87-108">Важные моменты, которые необходимо знать об имитации атак **brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="0aa87-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="0aa87-109">Если в целевой учетной записи включена MFA и пароль был угашен правильно, учетная запись не будет скомпрометирована (второй фактор проверки подлинности будет неполным).</span><span class="sxs-lookup"><span data-stu-id="0aa87-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="0aa87-110">Размер файла пароля не может быть больше 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="0aa87-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="0aa87-111">Используйте один пароль в строке и включайте пустую строку (возвращение вагона) после последнего пароля в списке.</span><span class="sxs-lookup"><span data-stu-id="0aa87-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="0aa87-112">Важные моменты, которые необходимо знать о **симуляции приложении к** фишингу копий:</span><span class="sxs-lookup"><span data-stu-id="0aa87-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="0aa87-113">По дизайну вы не можете предоставить настраиваемую ценность для **URL-адреса сервера фишинговых входов.**</span><span class="sxs-lookup"><span data-stu-id="0aa87-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="0aa87-114">Если получатель использует надстройку [Enable the Report Message](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) для сообщения о фишинге, вы можете не получать оповещений о сообщении (так как это имитация атаки).</span><span class="sxs-lookup"><span data-stu-id="0aa87-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="0aa87-115">Отчеты. После завершения смоделированной атаки можно нажать **кнопку Сведения** о атаке, чтобы увидеть отчет.</span><span class="sxs-lookup"><span data-stu-id="0aa87-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="0aa87-116">Подробные инструкции и новые функции в симуляторе атак см. в [Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="0aa87-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

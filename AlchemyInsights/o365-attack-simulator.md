---
title: Имитатор атак 2681 в Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801564"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="d78dd-102">Симулятор атак в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d78dd-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="d78dd-103">Вы не используете симулятор атак?</span><span class="sxs-lookup"><span data-stu-id="d78dd-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="d78dd-104">Для работы с симулятором атак требуется **защитник Майкрософт для Office 365, план 2 (ATP) (план 2)** или **Office 365 корпоративный** ~.</span><span class="sxs-lookup"><span data-stu-id="d78dd-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="d78dd-105">Симулятор атак **не** включен в защитник Майкрософт для Office 365, план 1 (ATP, план 1), Office 365 корпоративный E3 или любые приложения Microsoft 365 для бизнес-подписок.</span><span class="sxs-lookup"><span data-stu-id="d78dd-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="d78dd-106">Для учетной записи, используемой для запуска имитации атак, требуются разрешения администратора глобального администратора или безопасности, а также многофакторную проверку подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="d78dd-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="d78dd-107">Дополнительные сведения о требованиях к эмулятору атак приведены в [этой статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d78dd-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="d78dd-108">Важные сведения об управлении атаками **пароля методом грубой силы** :</span><span class="sxs-lookup"><span data-stu-id="d78dd-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="d78dd-109">Если для целевой учетной записи включен протокол MFA и правильно выбран пароль, то учетная запись не будет отображаться как скомпрометированная (второй фактор проверки подлинности будет неполным).</span><span class="sxs-lookup"><span data-stu-id="d78dd-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="d78dd-110">Размер файла паролей не может превышать 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="d78dd-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="d78dd-111">Используйте один пароль для каждой строки и включите пустую строку (возврат каретки) после последнего пароля в списке.</span><span class="sxs-lookup"><span data-stu-id="d78dd-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="d78dd-112">Важные сведения о имитации имитации **спеар фишинг** -подключения:</span><span class="sxs-lookup"><span data-stu-id="d78dd-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="d78dd-113">По дизайну невозможно предоставить настраиваемое значение для **URL-адреса сервера входа в систему фишинга** .</span><span class="sxs-lookup"><span data-stu-id="d78dd-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="d78dd-114">Если получатель использует [надстройку "включение сообщения отчета](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " для сообщения о качестве фишинга, вы можете не получать оповещения для этого сообщения (так как это имитация атаки).</span><span class="sxs-lookup"><span data-stu-id="d78dd-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="d78dd-115">Отчеты: после завершения имитации атаки вы можете просмотреть отчет, щелкнув **сведения об атаках** .</span><span class="sxs-lookup"><span data-stu-id="d78dd-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="d78dd-116">Подробная информация о новых возможностях и новых возможностях в симуляторе атак приведена [в статье симулятор атак в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="d78dd-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

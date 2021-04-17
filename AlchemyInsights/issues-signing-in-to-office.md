---
title: Проблемы с входом в приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833052"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="700cb-102">Пустой экран регистрации в приложениях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="700cb-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="700cb-103">Чтобы устранить эту проблему, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="700cb-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="700cb-104">Установка последних обновлений [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="700cb-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="700cb-105">Сброс параметров Internet Explorer: Перейдите к средствам параметров Internet  >    >  **Advanced**  >  **Reset Internet Explorer Settings** (обратите внимание, что вы потеряете настраиваемые параметры), а затем попробуйте снова входить в Office.</span><span class="sxs-lookup"><span data-stu-id="700cb-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="700cb-106">Отключение Защитник Windows безопасности приложений (WDAG) или любого аналогичного брандмауэра или антивирусной программы:</span><span class="sxs-lookup"><span data-stu-id="700cb-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="700cb-107">В панели управления перейдите к **программам,** а затем выберите включить или отключить функции **Windows.**</span><span class="sxs-lookup"><span data-stu-id="700cb-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="700cb-108">Если Защитник Windows включена охрана приложений, попробуйте отключить ее.</span><span class="sxs-lookup"><span data-stu-id="700cb-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="700cb-109">**Примечание:** Возможно, потребуется перезапустить компьютер.</span><span class="sxs-lookup"><span data-stu-id="700cb-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="700cb-110">Убедитесь, что подключаемый модуль WAM Microsoft.AAD.BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не блокируется ни приложением, ни брандмауэром, ни антивирусной программой.</span><span class="sxs-lookup"><span data-stu-id="700cb-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="700cb-111">[Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="700cb-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="700cb-112">**Примечание:** Пути реестра Office 2016 изменились до 16.0.</span><span class="sxs-lookup"><span data-stu-id="700cb-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="700cb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="700cb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="700cb-114">Дополнительные сведения см. в документе Проблемы подключения при входе после обновления [office 2016 сборки 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="700cb-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
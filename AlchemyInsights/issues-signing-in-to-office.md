---
title: Проблемы с входом в приложения Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695300"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="29670-102">Пустой экран входа в приложения Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="29670-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="29670-103">Чтобы устранить эту проблему, попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="29670-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="29670-104">Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="29670-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="29670-105">Сброс параметров Internet Explorer: Откройте **меню Сервис**  >  **параметры Internet**  >  **Advanced**  >  **Explorer дополнительно сбросить параметры Internet Explorer** (Обратите внимание, что настраиваемые параметры будут утрачены), а затем попробуйте войти в Office снова.</span><span class="sxs-lookup"><span data-stu-id="29670-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="29670-106">Отключите приложение Application Guard в Защитнике Windows (ВДАГ) или аналогичное брандмауэр или антивирусную программу:</span><span class="sxs-lookup"><span data-stu-id="29670-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="29670-107">В панели управления откройте раздел **программы**, а затем выберите пункт **Включение или отключение компонентов Windows**.</span><span class="sxs-lookup"><span data-stu-id="29670-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="29670-108">Если включено Application Guard в Защитнике Windows, попробуйте отключить его.</span><span class="sxs-lookup"><span data-stu-id="29670-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="29670-109">**Примечание:** Может потребоваться перезагрузка компьютера.</span><span class="sxs-lookup"><span data-stu-id="29670-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="29670-110">Убедитесь, что [подключаемый модуль](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. БРОКЕРПЛУГИН AAD вам не блокируется каким-либо приложением или брандмауэром/антивирусной программой.</span><span class="sxs-lookup"><span data-stu-id="29670-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="29670-111">[Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="29670-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="29670-112">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="29670-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="29670-113">(Пример: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="29670-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="29670-114">Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="29670-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
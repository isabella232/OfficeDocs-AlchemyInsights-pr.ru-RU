---
title: Проблемы с входом в приложения Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938319"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="9a6ee-102">Пустой экран входа в приложения Office</span><span class="sxs-lookup"><span data-stu-id="9a6ee-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="9a6ee-103">Чтобы устранить эту проблему, попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="9a6ee-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9a6ee-104">Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9a6ee-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9a6ee-105">Сброс параметров Internet Explorer: Откройте **меню Сервис** > **Параметры** > Internet Explorer**Дополнительно** > **сбросить параметры Internet Explorer** (Обратите внимание, что настраиваемые параметры будут утрачены), а затем попробуйте войти в Office снова.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9a6ee-106">Отключите приложение Application Guard в Защитнике Windows (ВДАГ) или аналогичное брандмауэр или антивирусную программу:</span><span class="sxs-lookup"><span data-stu-id="9a6ee-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9a6ee-107">В панели управления откройте раздел **программы**, а затем выберите пункт **Включение или отключение компонентов Windows**.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9a6ee-108">Если включено Application Guard в Защитнике Windows, попробуйте отключить его.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9a6ee-109">**Примечание:** Может потребоваться перезагрузка компьютера.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9a6ee-110">Убедитесь, что [подключаемый модуль](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. БРОКЕРПЛУГИН AAD вам не блокируется каким-либо приложением или брандмауэром/антивирусной программой.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9a6ee-111">[Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9a6ee-112">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="9a6ee-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9a6ee-113">(Пример: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9a6ee-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9a6ee-114">Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9a6ee-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
---
title: Проблемы с входом в приложения Microsoft 365
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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579878"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="2e928-102">Исправление приложений Microsoft 365 "доверенный платформенный модуль вашего компьютера не работает должным образом" сообщение</span><span class="sxs-lookup"><span data-stu-id="2e928-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="2e928-103">Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="2e928-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="2e928-104">Установите последние обновления для [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2e928-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2e928-105">[Очистите учетные данные Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="2e928-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2e928-106">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="2e928-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2e928-107">(Пример: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2e928-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2e928-108">Попытайтесь выполнить [процесс восстановления пользователей](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , чтобы исправить ошибки ДОВЕРЕНного платформенного модуля.</span><span class="sxs-lookup"><span data-stu-id="2e928-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="2e928-109">Задайте Енаблеадал = 0, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="2e928-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="2e928-110">Щелкните правой кнопкой мыши Windows Пуск, выберите команду **выполнить**, введите **regedit**и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="2e928-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="2e928-111">Выберите **Да** , чтобы разрешить редактору реестра вносить изменения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2e928-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="2e928-112">В редакторе реестра добавьте значение DWORD **енаблеадал** с параметром **0** в раздел HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="2e928-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="2e928-113">Дополнительные сведения см. [в статье проблемы с подключением при входе после обновления до Office 2016 Build 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2e928-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
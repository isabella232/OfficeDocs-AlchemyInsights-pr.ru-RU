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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833017"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d20aa-102">Исправление приложения Microsoft 365 "Модуль доверенных платформ компьютера не функционирует должным образом" сообщение</span><span class="sxs-lookup"><span data-stu-id="d20aa-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d20aa-103">Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="d20aa-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d20aa-104">Установка последних обновлений [для Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="d20aa-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d20aa-105">[Очистить учетные данные Office с](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) помощью Диспетчер учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="d20aa-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d20aa-106">**Примечание:** Пути реестра Office 2016 изменились до 16.0.</span><span class="sxs-lookup"><span data-stu-id="d20aa-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d20aa-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d20aa-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d20aa-108">Попробуйте [процесс восстановления пользователей,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) чтобы устранить сбои в работе модуля доверенных платформ (TPM).</span><span class="sxs-lookup"><span data-stu-id="d20aa-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d20aa-109">Установите EnableADAL = 0 с помощью следующих действий:</span><span class="sxs-lookup"><span data-stu-id="d20aa-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d20aa-110">Щелкните правой кнопкой Запуска Windows, выберите **выполнить,** введите **regedit,** а затем выберите **ОК.**</span><span class="sxs-lookup"><span data-stu-id="d20aa-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d20aa-111">Выберите **Да,** чтобы разрешить редактору реестра вносить изменения в устройство.</span><span class="sxs-lookup"><span data-stu-id="d20aa-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d20aa-112">В редакторе реестра добавьте значение DWORD **EnableADAL** с параметром **0** в HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d20aa-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d20aa-113">Дополнительные сведения см. в документе Проблемы подключения при входе после обновления [office 2016 сборки 16.0.7967 в Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="d20aa-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>
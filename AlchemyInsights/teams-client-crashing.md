---
title: Сбой клиента Teams?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826284"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="efb52-102">Сбой клиента Teams?</span><span class="sxs-lookup"><span data-stu-id="efb52-102">Teams client crashing?</span></span>

<span data-ttu-id="efb52-103">Если ваш клиент Teams дает сбой, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="efb52-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="efb52-104">Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.</span><span class="sxs-lookup"><span data-stu-id="efb52-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="efb52-105">убедитесь в доступности всех [URL-адресов Microsoft 365 и диапазонов адресов](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="efb52-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="efb52-106">Войдите в систему с учетной записью администратора клиента и проверьте [панель мониторинга работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев и снижения качества обслуживания.</span><span class="sxs-lookup"><span data-stu-id="efb52-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="efb52-107">Удалите и повторно установите приложение Teams (ссылка)</span><span class="sxs-lookup"><span data-stu-id="efb52-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="efb52-108">Перейдите в папку %appdata%\Microsoft\teams\ на вашем компьютере и удалите все файлы в этой папке.</span><span class="sxs-lookup"><span data-stu-id="efb52-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="efb52-109">[Скачайте и установите приложение Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy) и, если это возможно, установите Teams от имени администратора (щелкните правой кнопкой мыши установщик Teams и выберите пункт «Запуск от имени администратора»).</span><span class="sxs-lookup"><span data-stu-id="efb52-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="efb52-110">Если в работе клиента Teams по-прежнему возникают сбои, сможете ли вы воспроизвести проблему?</span><span class="sxs-lookup"><span data-stu-id="efb52-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="efb52-111">Если да:</span><span class="sxs-lookup"><span data-stu-id="efb52-111">If so:</span></span>

1. <span data-ttu-id="efb52-112">Запишите действия, используя средство записи действий.</span><span class="sxs-lookup"><span data-stu-id="efb52-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="efb52-113">Закройте все ненужные приложения и приложения, работающие с конфиденциальной информацией.</span><span class="sxs-lookup"><span data-stu-id="efb52-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="efb52-114">Запустите средство записи действий и воспроизведите проблему, выполнив вход в затронутую учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="efb52-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="efb52-115">[Соберите журналы команд, которые фиксируют записанные шаги воспроизведения](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="efb52-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="efb52-116">**Примечание**: Убедитесь в том, что вы записали адрес для входа в систему затронутых пользователей.</span><span class="sxs-lookup"><span data-stu-id="efb52-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="efb52-117">Соберите сведения о дампе и/или сведения о контейнере ошибки (Windows).</span><span class="sxs-lookup"><span data-stu-id="efb52-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="efb52-118">Запустите Windows PowerShell на компьютере, на котором происходит сбой, и выполните следующие команды:</span><span class="sxs-lookup"><span data-stu-id="efb52-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="efb52-119">Вложите файл в ваше обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="efb52-119">Attach the file to your support case.</span></span>

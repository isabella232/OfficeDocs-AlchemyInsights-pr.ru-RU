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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187734"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="d5b65-102">Сбой клиента Teams?</span><span class="sxs-lookup"><span data-stu-id="d5b65-102">Teams client crashing</span></span>

<span data-ttu-id="d5b65-103">Если ваш клиент Teams дает сбой, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="d5b65-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="d5b65-104">Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.</span><span class="sxs-lookup"><span data-stu-id="d5b65-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="d5b65-105">убедитесь в доступности всех [URL-адресов Microsoft 365 и диапазонов адресов](/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="d5b65-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="d5b65-106">Войдите в систему с учетной записью администратора клиента и проверьте [панель мониторинга работоспособности службы](/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев и снижения качества обслуживания.</span><span class="sxs-lookup"><span data-stu-id="d5b65-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="d5b65-107">Удалите и повторно установите приложение Teams</span><span class="sxs-lookup"><span data-stu-id="d5b65-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="d5b65-108">Перейдите в папку %appdata%\Microsoft\Teams\ на вашем компьютере и удалите все файлы в этой папке.</span><span class="sxs-lookup"><span data-stu-id="d5b65-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="d5b65-109">[Скачайте и установите приложение Teams](https://www.microsoft.com/microsoft-teams/download-app) и, если это возможно, установите Teams от имени администратора (щелкните правой кнопкой мыши установщик Teams и выберите пункт **Запуск от имени администратора**).</span><span class="sxs-lookup"><span data-stu-id="d5b65-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="d5b65-110">Если в работе клиента Teams по-прежнему возникают сбои, попробуйте воспроизвести проблему.</span><span class="sxs-lookup"><span data-stu-id="d5b65-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="d5b65-111">Если можешь...</span><span class="sxs-lookup"><span data-stu-id="d5b65-111">If you can:</span></span>

1. <span data-ttu-id="d5b65-112">Запишите действия, используя средство записи действий.</span><span class="sxs-lookup"><span data-stu-id="d5b65-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="d5b65-113">Закройте все ненужные приложения и приложения, работающие с конфиденциальной информацией.</span><span class="sxs-lookup"><span data-stu-id="d5b65-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="d5b65-114">Запустите средство записи действий и воспроизведите проблему, выполнив вход в затронутую учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="d5b65-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="d5b65-115">[Соберите журналы команд, которые фиксируют записанные шаги воспроизведения](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="d5b65-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="d5b65-116">**Примечание**: Убедитесь в том, что вы записали адрес для входа в систему затронутых пользователей.</span><span class="sxs-lookup"><span data-stu-id="d5b65-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="d5b65-117">Соберите сведения о дампе и/или сведения о контейнере ошибки (Windows).</span><span class="sxs-lookup"><span data-stu-id="d5b65-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="d5b65-118">Запустите Windows PowerShell на компьютере, на котором происходит сбой, и выполните следующие команды (нажимая после каждой кнопку ВВОД):</span><span class="sxs-lookup"><span data-stu-id="d5b65-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="d5b65-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="d5b65-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="d5b65-120">После того как текстовый файл будет создан и появится на экране, сохраните его и вложите в запрос на обслуживание.</span><span class="sxs-lookup"><span data-stu-id="d5b65-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 

---
title: Сбой клиента Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030675"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="95521-102">Сбой клиента Teams?</span><span class="sxs-lookup"><span data-stu-id="95521-102">Teams client crashing?</span></span>

<span data-ttu-id="95521-103">Если ваш клиент Teams дает сбой, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="95521-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="95521-104">Если вы используете классическое приложение Teams, [убедиться в том, что приложение Обновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)о.</span><span class="sxs-lookup"><span data-stu-id="95521-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="95521-105">Убедитесь, что все [URL-адреса и диапазоны адресов Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступны.</span><span class="sxs-lookup"><span data-stu-id="95521-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="95521-106">Войдите в систему под своей учетной записью администратора и проверьте [панель мониторинга работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health), чтобы убедиться в отсутствии перебоев или ухудшении качества обслуживания.</span><span class="sxs-lookup"><span data-stu-id="95521-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="95521-107">В качестве последнего шага вы можете попытаться очистить кеш клиента вашего Teams:</span><span class="sxs-lookup"><span data-stu-id="95521-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="95521-108">Полностью выйдите из настольного клиента Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="95521-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="95521-109">Можно щелкнуть правой кнопкой мыши **Teams** в области значков и выбрать команду **закрыть**или запустить диспетчер задач и выполнить полное завершение процесса.</span><span class="sxs-lookup"><span data-stu-id="95521-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="95521-110">Перейдите в проводник и введите %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="95521-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="95521-111">Попав в каталог, вы увидите несколько следующих папок:</span><span class="sxs-lookup"><span data-stu-id="95521-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="95521-112">Из **кеша приложений** перейдите в кеш и удалите все файлы в расположении  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="95521-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="95521-113">Из **Blob_storage** удалите все файлы: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="95521-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="95521-114">Из **кэша** удалите все файлы: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="95521-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="95521-115">Из **баз данных** удалите все файлы: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="95521-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="95521-116">Из **GPUCache** удалите все файлы: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="95521-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="95521-117">Изнутри **IndexedDB** удалите файл .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="95521-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="95521-118">Из **локального хранилища** удалите все файлы:%appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="95521-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="95521-119">Наконец, из **tmp** удалите любой файл:%appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="95521-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="95521-120">Перезапустите клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="95521-120">Restart your Teams client.</span></span>

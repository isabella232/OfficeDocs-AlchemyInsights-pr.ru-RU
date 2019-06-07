---
title: Уровни разрешений SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760705"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="6d4fe-102">Проблемы с подключением SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="6d4fe-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="6d4fe-103">Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, попробуйте выполнить следующие распространенные решения.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="6d4fe-104">Шаг 1: Проверьте, обновлен ли SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="6d4fe-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="6d4fe-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="6d4fe-106">Пакет обновления 1 (SP1) для SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="6d4fe-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="6d4fe-107">Обновление для SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="6d4fe-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="6d4fe-108">Шаг 2: очистите файлы локального кэша</span><span class="sxs-lookup"><span data-stu-id="6d4fe-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="6d4fe-109">Закройте SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="6d4fe-110">На локальном компьютере перейдите к следующим папкам, чтобы удалить кэшированные файлы.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="6d4fe-111">Нажмите кнопку Пуск, запустите и удалите все файлы, найденные в каждом из указанных ниже расположений.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="6d4fe-112">%Аппдата%\микрософт\веб Server Екстенсионс\каче%Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="6d4fe-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="6d4fe-113">Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="6d4fe-114">Шаг 3: [Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="6d4fe-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="6d4fe-115">Шаг 4: Администраторы должны разрешить пользовательскому сценарию разрешить подключение SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="6d4fe-116">Подробное описание действий, примеры и рекомендации [](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)см.</span><span class="sxs-lookup"><span data-stu-id="6d4fe-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>



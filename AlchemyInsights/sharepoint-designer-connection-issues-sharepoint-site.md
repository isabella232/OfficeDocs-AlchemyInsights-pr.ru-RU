---
title: Проблемы с подключением SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051726"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="3053f-102">Проблемы с подключением SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="3053f-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="3053f-103">Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, воспользуйтесь следующими распространенными решениями.</span><span class="sxs-lookup"><span data-stu-id="3053f-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="3053f-104">Шаг 1: Убедитесь, что SharePoint Designer 2013 обновлен с помощью [SharePoint Designer с пакетом обновления 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [обновлением 2 августа 2016 для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="3053f-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="3053f-105">Шаг 2: очистите файлы локального кэша:</span><span class="sxs-lookup"><span data-stu-id="3053f-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="3053f-106">Закройте SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3053f-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="3053f-107">На локальном компьютере удалите все файлы, найденные в каждой из следующих папок.</span><span class="sxs-lookup"><span data-stu-id="3053f-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="3053f-108">%Аппдата%\микрософт\веб Server Екстенсионс\каче</span><span class="sxs-lookup"><span data-stu-id="3053f-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="3053f-109">%Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче</span><span class="sxs-lookup"><span data-stu-id="3053f-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="3053f-110">%усерпрофиле%\аппдата\локал\микрософт\вебситекаче</span><span class="sxs-lookup"><span data-stu-id="3053f-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="3053f-111">Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.</span><span class="sxs-lookup"><span data-stu-id="3053f-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="3053f-112">Шаг 3: [Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3053f-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="3053f-113">Шаг 4: администратору необходимо **Разрешить пользовательскому скрипту** в параметрах центра администрирования SharePoint разрешить подключение SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="3053f-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="3053f-114">Для [получения](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="3053f-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>



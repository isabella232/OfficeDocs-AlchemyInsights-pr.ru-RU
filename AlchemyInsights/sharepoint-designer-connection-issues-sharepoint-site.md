---
title: Проблемы с подключением SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840564"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7d7d7-102">Проблемы с подключением SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="7d7d7-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7d7d7-103">Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, воспользуйтесь следующими распространенными решениями.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="7d7d7-104">Шаг 1: Убедитесь, что SharePoint Designer 2013 обновлен с помощью [SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) с пакетом обновления 1 и [обновлением 2 августа 2016 для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="7d7d7-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="7d7d7-105">Шаг 2: очистите файлы локального кэша:</span><span class="sxs-lookup"><span data-stu-id="7d7d7-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="7d7d7-106">Закройте SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="7d7d7-107">На локальном компьютере удалите все файлы, найденные в каждой из следующих папок.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="7d7d7-108">%Аппдата%\микрософт\веб Server Екстенсионс\каче</span><span class="sxs-lookup"><span data-stu-id="7d7d7-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="7d7d7-109">%Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче</span><span class="sxs-lookup"><span data-stu-id="7d7d7-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="7d7d7-110">%Усерпрофиле%\аппдата\локал\микрософт\вебситекаче</span><span class="sxs-lookup"><span data-stu-id="7d7d7-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="7d7d7-111">Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7d7d7-112">Шаг 3: [Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="7d7d7-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="7d7d7-113">Шаг 4: администратору необходимо **Разрешить пользовательскому скрипту** в параметрах центра администрирования SharePoint разрешить подключение SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="7d7d7-114">Для [](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="7d7d7-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>



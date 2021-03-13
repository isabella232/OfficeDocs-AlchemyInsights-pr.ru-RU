---
title: Удаление фоновой службы Поиска (Майкрософт) в Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753442"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="8090d-102">Удаление фоновой службы Поиска (Майкрософт) в Bing</span><span class="sxs-lookup"><span data-stu-id="8090d-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="8090d-103">Чтобы удалить фоновую службу Поиска (Майкрософт) в Bing, попробуйте следующие решения.</span><span class="sxs-lookup"><span data-stu-id="8090d-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="8090d-104">Чтобы вернуться к исходным настройкам поисковой системы, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="8090d-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="8090d-105">а.</span><span class="sxs-lookup"><span data-stu-id="8090d-105">a.</span></span> <span data-ttu-id="8090d-106">Переведите переключатель **Использовать Bing в качестве поисковой системы по умолчанию[ в положение](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)Выкл**.</span><span class="sxs-lookup"><span data-stu-id="8090d-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="8090d-107">б.</span><span class="sxs-lookup"><span data-stu-id="8090d-107">b.</span></span> <span data-ttu-id="8090d-108">[Перейдите в Центр администрирования Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) и снимите флажок с параметра, влияющего на всех пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="8090d-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="8090d-109">Чтобы удалить фоновую службу с отдельного устройства, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="8090d-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="8090d-110">а.</span><span class="sxs-lookup"><span data-stu-id="8090d-110">a.</span></span> <span data-ttu-id="8090d-111">Выберите **Панель управления > Программы > Программы и компоненты**.</span><span class="sxs-lookup"><span data-stu-id="8090d-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="8090d-112">б.</span><span class="sxs-lookup"><span data-stu-id="8090d-112">b.</span></span> <span data-ttu-id="8090d-113">Щелкните правой кнопкой мыши **Поиск (Майкрософт) в Bing** в списке установленных программ и нажмите **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="8090d-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="8090d-114">Чтобы удалить фоновую службу с нескольких устройств в организации, войдите в систему с учетной записью администратора и запустите следующую команду в сценарии.</span><span class="sxs-lookup"><span data-stu-id="8090d-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`

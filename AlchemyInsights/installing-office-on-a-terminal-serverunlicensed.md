---
title: Установка Office на сервере терминалов — Нелицензировано
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381742"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="4a2c6-102">Установка Office на сервере терминалов</span><span class="sxs-lookup"><span data-stu-id="4a2c6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="4a2c6-103">Для развертывания Office 365 профессиональный плюс на Windows Server с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:</span><span class="sxs-lookup"><span data-stu-id="4a2c6-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="4a2c6-104">Вы должны иметь план Office 365, включающий Office 365 профессиональный плюс, например Office 365 Enterprise E3 или Enterprise "\".</span><span class="sxs-lookup"><span data-stu-id="4a2c6-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="4a2c6-105">Планы Office 365 для бизнеса и Office 365 бизнес премиум не включают Office 365 профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="4a2c6-106">Необходимо включить активацию на [общем компьютере](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4a2c6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="4a2c6-107">Если вы хотите установить Office 365 профессиональный плюс для RDS на портале Office 365, \* \*, *где используются параметры установки по умолчанию* \* \*, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="4a2c6-108">Проверьте, какой план Office 365 у вас есть.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="4a2c6-109">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="4a2c6-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="4a2c6-110">При необходимости переключитесь на другой план Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="4a2c6-111">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="4a2c6-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="4a2c6-112">Если Office уже установлен на сервере RDS с помощью других планов Office 365, удалите его.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="4a2c6-113">Например, с помощью панели \> управления удалите программу.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="4a2c6-114">Удаление с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="4a2c6-115">На сервере RDS Войдите на портал Office 365 с помощью учетной записи администратора и [установите Office 365 профессиональный плюс](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="4a2c6-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="4a2c6-116">После установки Office \* \* *не открывайте и не входите в* приложение Office \* \*.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="4a2c6-117">На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="4a2c6-118">Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду выполнить.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="4a2c6-119">В поле Открыть введите regedit \*\*\*\* и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="4a2c6-120">Выберите Да, если будет предложено разрешить редактору реестра вносить изменения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="4a2c6-121">В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе хкэй_локал_мачине\софтваре\микрософт \оффице\кликкторун\конфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4a2c6-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="4a2c6-122">На сервере RDS \* \* *выполните вход в качестве конечного пользователя* \* \* и [Убедитесь, что активация на общем компьютере включена для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="4a2c6-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="4a2c6-123">Для получения дополнительных сведений о предварительных требованиях и инструкциях по настройке для настраиваемых установок с помощью средства развертывания Office, ознакомьтесь со статьей [развертывание office 365 профессиональный плюс с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="4a2c6-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="4a2c6-124">Устранение ошибок, связанных с активацией на общедоступном компьютере, можно найти в статье [Устранение неполадок при активации на общем компьютере для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4a2c6-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
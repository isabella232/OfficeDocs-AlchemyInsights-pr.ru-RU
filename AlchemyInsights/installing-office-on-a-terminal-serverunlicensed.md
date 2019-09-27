---
title: Установка Office на сервере терминалов — Нелицензировано
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205422"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="bd4fd-102">Установка Office на сервере терминалов</span><span class="sxs-lookup"><span data-stu-id="bd4fd-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="bd4fd-103">Для развертывания Office 365 профессиональный плюс на Windows Server с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:</span><span class="sxs-lookup"><span data-stu-id="bd4fd-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="bd4fd-104">Вы должны иметь план Office 365, включающий Office 365 профессиональный плюс, например Office 365 Enterprise E3 или Enterprise "\".</span><span class="sxs-lookup"><span data-stu-id="bd4fd-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="bd4fd-105">Планы Office 365 для бизнеса и Office 365 бизнес премиум не включают Office 365 профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="bd4fd-106">Необходимо включить [активацию на общем компьютере](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="bd4fd-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="bd4fd-107">Если вы хотите установить Office 365 профессиональный плюс в RDS из центра администрирования Microsoft 365, ***который использует параметры установки по умолчанию***, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="bd4fd-108">Вы также можете скачать и запустить [Помощник по поддержке и восстановлению Майкрософт](https://aka.ms/SaRA_OfficeSCA_M365Portal) , чтобы установить Office 365 профессиональный плюс в режиме активации на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="bd4fd-109">Проверьте, какой план Office 365 у вас есть.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="bd4fd-110">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="bd4fd-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="bd4fd-111">При необходимости переключитесь на другой план Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="bd4fd-112">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="bd4fd-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="bd4fd-113">Если Office уже установлен на сервере RDS с помощью других планов Office 365, удалите его.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="bd4fd-114">Например, с помощью панели \> управления удалите программу.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="bd4fd-115">Удаление с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="bd4fd-116">На сервере RDS Войдите в центр администрирования Microsoft 365 с учетной записью администратора и [установите Office 365 профессиональный плюс](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="bd4fd-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="bd4fd-117">После установки Office ***не открывайте и не входите*** в приложения Office.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="bd4fd-118">На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="bd4fd-119">Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду выполнить.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="bd4fd-120">В поле Открыть введите **regedit**и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="bd4fd-121">Выберите Да, если будет предложено разрешить редактору реестра вносить изменения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="bd4fd-122">В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \оффице\кликкторун\конфигуратион.</span><span class="sxs-lookup"><span data-stu-id="bd4fd-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="bd4fd-123">На сервере RDS ***выполните вход в качестве конечного пользователя*** и [Убедитесь, что активация на общем компьютере включена для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="bd4fd-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="bd4fd-124">Для получения дополнительных сведений о предварительных требованиях и инструкциях по настройке для настраиваемых установок с помощью средства развертывания Office, ознакомьтесь со статьей [развертывание office 365 профессиональный плюс с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="bd4fd-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="bd4fd-125">Устранение ошибок, связанных с активацией на общедоступном компьютере, можно найти в статье [Устранение неполадок при активации на общем компьютере для Office 365 профессиональный плюс](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="bd4fd-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
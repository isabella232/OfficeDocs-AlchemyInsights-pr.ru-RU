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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508641"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="cc4e7-102">Установка Office на сервере терминалов</span><span class="sxs-lookup"><span data-stu-id="cc4e7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="cc4e7-103">Для развертывания приложений Microsoft 365 для предприятий в Windows Server с помощью служб удаленных рабочих столов (RDS), ранее именуемых службами терминалов:</span><span class="sxs-lookup"><span data-stu-id="cc4e7-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="cc4e7-104">Вы должны иметь подписку на Microsoft 365, включающую приложения Майкрософт 365 для предприятий, например Office 365 Enterprise E3 или Enterprise "\".</span><span class="sxs-lookup"><span data-stu-id="cc4e7-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="cc4e7-105">Приложения Microsoft 365 для бизнеса и Microsoft 365 для планов бизнеса Premium не включают приложения Microsoft 365 для предприятия.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="cc4e7-106">Необходимо включить [активацию на общем компьютере](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="cc4e7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="cc4e7-107">Если вы хотите установить приложения Microsoft 365 для Enterprise в RDS из центра администрирования Майкрософт 365, ***использующего параметры установки по умолчанию***, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="cc4e7-108">Вы также можете скачать и запустить [Помощник по поддержке и восстановлению Майкрософт](https://aka.ms/SaRA_OfficeSCA_M365Portal) для установки приложений Microsoft 365 для предприятий в режиме активации на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="cc4e7-109">Проверьте, что у вас есть подписка на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="cc4e7-110">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="cc4e7-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="cc4e7-111">При необходимости переключитесь на другую подписку Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="cc4e7-112">Узнайте, как</span><span class="sxs-lookup"><span data-stu-id="cc4e7-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="cc4e7-113">Если Office уже установлен на сервере RDS с использованием других подписок Microsoft 365, удалите его.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="cc4e7-114">Например, с помощью панели управления \> удалите программу.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="cc4e7-115">Удаление с помощью [помощника по поддержке и восстановлению Майкрософт](https://aka.ms/SARA-OfficeUninstall-Alchemy) , если у вас возникли проблемы.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="cc4e7-116">На сервере RDS Войдите в центр администрирования Microsoft 365 с учетной записью администратора и [установите приложения Microsoft 365 для предприятия](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="cc4e7-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="cc4e7-117">После установки Office ***не открывайте и не входите*** в приложения Office.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="cc4e7-118">На сервере RDS Включите активацию на общем компьютере, отредактировав реестр, выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="cc4e7-119">Щелкните правой кнопкой мыши кнопку Windows в левом нижнем углу экрана и выберите команду выполнить.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="cc4e7-120">В поле Открыть введите **regedit**и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="cc4e7-121">Выберите Да, если будет предложено разрешить редактору реестра вносить изменения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="cc4e7-122">В редакторе реестра добавьте строковое значение **SharedComputerLicensing** с параметром 1 в разделе HKEY_LOCAL_MACHINE \софтваре\микрософт \оффице\кликкторун\конфигуратион.</span><span class="sxs-lookup"><span data-stu-id="cc4e7-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="cc4e7-123">***Выполните вход в качестве конечного пользователя*** на сервере RDS и [Убедитесь, что активация на общем компьютере включена для приложений Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="cc4e7-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="cc4e7-124">Для получения дополнительных сведений о предварительных требованиях и инструкциях по настройке для настраиваемых установок с помощью средства развертывания Office, ознакомьтесь со статьей [развертывание приложений Microsoft 365 для предприятий с помощью служб удаленных рабочих столов](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="cc4e7-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="cc4e7-125">Устранение ошибок, связанных с активацией на общедоступном компьютере, можно найти в [статье Устранение неполадок, связанных с активацией на общем компьютере для приложений Microsoft 365 для предприятий](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="cc4e7-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  
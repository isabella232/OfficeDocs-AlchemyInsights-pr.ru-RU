---
title: Развертывание приложений Microsoft 365 для предприятия для общего использования в RDS, Terminal Server или VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200686"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="78437-102">Развертывание приложений Microsoft 365 для предприятия для общего использования в RDS, Terminal Server или VDI</span><span class="sxs-lookup"><span data-stu-id="78437-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="78437-103">Развертывание приложений Microsoft 365 для предприятия с использованием служб удаленного рабочего стола (RDS), ранее именуемой службами терминалов:</span><span class="sxs-lookup"><span data-stu-id="78437-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="78437-104">Необходимо иметь план Microsoft 365 для бизнеса или план Office 365, который включает приложения Microsoft 365 для предприятия, такие как Office 365 Enterprise E3 или Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="78437-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="78437-105">Планы Microsoft 365 Apps для бизнеса и Microsoft 365 Business Standard не включают приложения Microsoft 365 для предприятия.</span><span class="sxs-lookup"><span data-stu-id="78437-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="78437-106">Необходимо включить [активацию общего компьютера.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="78437-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="78437-107">Вы также можете скачать и запустить [помощник по поддержке и](https://aka.ms/SaRA_OfficeSCA_M365Portal) восстановлению Майкрософт для установки приложений Microsoft 365 для предприятия в режиме активации общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="78437-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="78437-108">Дополнительные сведения о необходимых предпосылках, инструкциях по установке и руководстве по настраиваемым установкам с помощью средства развертывания Office см. в рублях [Deploy Microsoft 365 Apps для](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)предприятия с помощью служб удаленного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="78437-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="78437-109">Устранение ошибок, связанных с активацией общего компьютера:</span><span class="sxs-lookup"><span data-stu-id="78437-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="78437-110">См. [раздел Устранение неполадок с активацией общих компьютеров для Microsoft 365 Apps для предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="78437-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="78437-111">См. статью [Сброс приложений Microsoft 365 до корпоративного состояния активации](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="78437-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="78437-112">Если вы хотите установить Microsoft 365 Apps для предприятия на RDS из центра администрирования Microsoft 365, который использует параметры установки по умолчанию, используйте следующие действия:</span><span class="sxs-lookup"><span data-stu-id="78437-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="78437-113">Проверьте, какая у вас подписка.</span><span class="sxs-lookup"><span data-stu-id="78437-113">Check what subscription you have.</span></span> <span data-ttu-id="78437-114">[Инструкции.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="78437-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="78437-115">При необходимости переключение на другую подписку.</span><span class="sxs-lookup"><span data-stu-id="78437-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="78437-116">[Инструкции.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="78437-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="78437-117">Если Office уже установлен на сервере RDS с помощью любых других подписок Майкрософт, удалить его.</span><span class="sxs-lookup"><span data-stu-id="78437-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="78437-118">Например, при помощи панели **управления** удалить программу  >  .</span><span class="sxs-lookup"><span data-stu-id="78437-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="78437-119">Если у вас проблемы, удалить с помощью [помощника по](https://aka.ms/SARA-OfficeUninstall-Alchemy) поддержке и восстановлению Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="78437-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="78437-120">На сервере RDS впишитесь в центр администрирования Microsoft 365 с учетной записью администратора и установите [приложения Microsoft 365 для предприятия.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="78437-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="78437-121">После установки Office не открывайтесь и не ***впишитесь в*** приложения Office.</span><span class="sxs-lookup"><span data-stu-id="78437-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="78437-122">На сервере RDS включить активацию общего компьютера, редактировать реестр, следуя следующим шагам:</span><span class="sxs-lookup"><span data-stu-id="78437-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="78437-123">Щелкните правой кнопкой Windows в нижнем левом углу экрана и выберите **Run**.</span><span class="sxs-lookup"><span data-stu-id="78437-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="78437-124">В поле Открыть введите команду **regedit** и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="78437-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="78437-125">Выберите **Да** при запросе разрешить редактору реестра вносить изменения на устройство.</span><span class="sxs-lookup"><span data-stu-id="78437-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="78437-126">В редакторе реестра добавьте строковую величину **SharedComputerLicensing** с параметром 1 в соответствии с HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="78437-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="78437-127">На сервере RDS  включайся как конечный пользователь и убедитесь, что активация общего компьютера включена для Microsoft [365 Apps для предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="78437-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

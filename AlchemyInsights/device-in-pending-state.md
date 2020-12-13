---
title: Устройство находится в состоянии ожидания
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652244"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="befd8-102">Устройство находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="befd8-102">Device in pending state</span></span>

<span data-ttu-id="befd8-103">**Необходимые условия:**</span><span class="sxs-lookup"><span data-stu-id="befd8-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="befd8-104">Если вы настраивали регистрацию устройств в первый раз, убедитесь, что вы рассмотрели введение в управление устройствами в [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) которое поможет вам получить устройства под управлением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="befd8-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="befd8-105">Если вы регистрируете устройства непосредственно в Azure AD и регистрируете их в Intune, вам [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) необходимо убедиться, что вы настроили [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и сначала настроили лицензирование.</span><span class="sxs-lookup"><span data-stu-id="befd8-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="befd8-106">Убедитесь, что вы уполномочены выполнять операции в Azure AD и локальной службе AD.</span><span class="sxs-lookup"><span data-stu-id="befd8-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="befd8-107">Только глобальный администратор в Azure AD может управлять настройками регистрации устройств.</span><span class="sxs-lookup"><span data-stu-id="befd8-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="befd8-108">Кроме того, при настройке автоматической регистрации в локальной службе Active Directory необходимо быть администратором Active Directory и AD FS (если это возможно).</span><span class="sxs-lookup"><span data-stu-id="befd8-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="befd8-109">Для регистрации гибридного присоединить Azure AD устройства должны быть в корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="befd8-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="befd8-110">Она также работает по VPN, но есть некоторые оговорки.</span><span class="sxs-lookup"><span data-stu-id="befd8-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="befd8-111">Мы узнали, что клиентам нужна помощь по устранению неполадок при регистрации гибридного присоединиться к Azure AD в условиях удаленной работы.</span><span class="sxs-lookup"><span data-stu-id="befd8-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="befd8-112">**Облачная среда проверки подлинности (с помощью синхронизации и сквозной проверки подлинности паролей Azure AD)**</span><span class="sxs-lookup"><span data-stu-id="befd8-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="befd8-113">Этот процесс регистрации также называется "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="befd8-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="befd8-114">Вот разбивка того, что происходит во время регистрации:</span><span class="sxs-lookup"><span data-stu-id="befd8-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="befd8-115">Windows 10 обнаруживает запись точки подключения службы (SCP) при входе пользователя на устройство.</span><span class="sxs-lookup"><span data-stu-id="befd8-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="befd8-116">Устройство сначала пытается получить сведения о клиенте из клиентского SCP в реестре [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="befd8-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="befd8-117">Дополнительные сведения см. в [документе.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="befd8-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="befd8-118">Если происходит сбой, устройство взаимодействует с локальной службой Active Directory для получения сведений о клиенте из SCP.</span><span class="sxs-lookup"><span data-stu-id="befd8-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="befd8-119">Чтобы проверить SCP, обратитесь к этому [документу.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)</span><span class="sxs-lookup"><span data-stu-id="befd8-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="befd8-120">Для начальной проверки рекомендуется включить SCP в Active Directory и использовать только клиентский SCP.</span><span class="sxs-lookup"><span data-stu-id="befd8-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="befd8-121">Windows 10 пытается связаться с Azure AD в контексте системы для проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="befd8-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="befd8-122">Вы можете проверить, может ли устройство получить доступ к ресурсам Майкрософт в системной учетной записи с помощью скрипта подключения для регистрации [тестовых устройств.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)</span><span class="sxs-lookup"><span data-stu-id="befd8-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="befd8-123">Windows 10 создает самозаверяяя сертификат и сохраняет его под объектом компьютера в локальной службе Active Directory.</span><span class="sxs-lookup"><span data-stu-id="befd8-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="befd8-124">Для этого требуется прямой просмотр контроллера домена.</span><span class="sxs-lookup"><span data-stu-id="befd8-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="befd8-125">Объект устройства с сертификатом синхронизируется с Azure AD через Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="befd8-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="befd8-126">По умолчанию цикл синхронизации каждые 30 минут, но он зависит от конфигурации Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="befd8-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="befd8-127">Дополнительные сведения можно получить в этом [документе.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)</span><span class="sxs-lookup"><span data-stu-id="befd8-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="befd8-128">На этом этапе вы сможете увидеть устройствотемы в состоянии "Ожидание" в blade устройства портала Azure.</span><span class="sxs-lookup"><span data-stu-id="befd8-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="befd8-129">При следующем входе пользователя в Windows 10 регистрация будет завершена.</span><span class="sxs-lookup"><span data-stu-id="befd8-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="befd8-130">Если вы подключены к VPN и при входе или входе в систему подключение к домену прерывается, регистрацию можно запускать вручную.</span><span class="sxs-lookup"><span data-stu-id="befd8-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="befd8-131">Для этого выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="befd8-131">To do that:</span></span>
    >
    > <span data-ttu-id="befd8-132">`dsregcmd /join`Выдайте локальное запрос администратора или удаленно через PSExec на компьютере.</span><span class="sxs-lookup"><span data-stu-id="befd8-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="befd8-133">Пример: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="befd8-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="befd8-134">Распространенные проблемы с регистрацией устройств Azure Active Directory см. в часто [задаваемом вопросе о устройствах.](https://docs.microsoft.com/azure/active-directory/devices/faq)</span><span class="sxs-lookup"><span data-stu-id="befd8-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>

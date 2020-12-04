---
title: Устранение проблем с ПРТ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571972"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="cb2be-102">Устранение проблем с ПРТ</span><span class="sxs-lookup"><span data-stu-id="cb2be-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="cb2be-103">Для того, чтобы любое устройство могло пройти проверку подлинности, оно должно быть полностью зарегистрировано и в хорошем состоянии и иметь возможность получить основной маркер обновления (ПРТ).</span><span class="sxs-lookup"><span data-stu-id="cb2be-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="cb2be-104">Для процесса регистрации присоединения к гибридной службе Azure AD необходимо, чтобы устройства направляться в корпоративную сеть.</span><span class="sxs-lookup"><span data-stu-id="cb2be-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="cb2be-105">Она также работает через VPN, но в ней есть некоторые предостережения.</span><span class="sxs-lookup"><span data-stu-id="cb2be-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="cb2be-106">Мы слышали о том, что вам потребуются рекомендации по устранению неисправностей гибридного процесса регистрации присоединения Azure AD в случае удаленных рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="cb2be-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="cb2be-107">Ниже приведена подразделение происходящих во время процесса регистрации.</span><span class="sxs-lookup"><span data-stu-id="cb2be-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="cb2be-108">**Облачная среда проверки подлинности (с использованием синхронизации хэша паролей Azure AD или сквозной проверки подлинности)**</span><span class="sxs-lookup"><span data-stu-id="cb2be-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="cb2be-109">Этот процесс регистрации также называется "соединение синхронизации".</span><span class="sxs-lookup"><span data-stu-id="cb2be-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="cb2be-110">Windows 10 обнаруживает запись SCP при входе пользователя на устройство.</span><span class="sxs-lookup"><span data-stu-id="cb2be-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="cb2be-111">Устройство сначала пытается получить сведения о клиенте из клиентской точки подключения на стороне клиента в реестре [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="cb2be-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="cb2be-112">Более подробную информацию можно узнать в этом [документе](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="cb2be-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="cb2be-113">В случае сбоя устройство обменивается данными с локальной службой Active Directory (AD), чтобы получить сведения о клиенте от точки подключения службы (SCP).</span><span class="sxs-lookup"><span data-stu-id="cb2be-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="cb2be-114">Чтобы проверить SCP, обратитесь к этому [документу](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="cb2be-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="cb2be-115">Мы рекомендуем включать SCP в Active Directory и только для первоначальной проверки, используя клиентскую точку входа на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="cb2be-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="cb2be-116">Windows 10 пытается общаться с Azure AD в контексте системы, чтобы пройти проверку подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb2be-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="cb2be-117">Вы можете проверить, может ли устройство получать доступ к ресурсам Майкрософт под учетной записью System с помощью сценария проверки подключения для Device Registration.</span><span class="sxs-lookup"><span data-stu-id="cb2be-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="cb2be-118">Windows 10 создает самозаверяющий сертификат и сохраняет его в объекте Computer в локальной службе AD.</span><span class="sxs-lookup"><span data-stu-id="cb2be-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="cb2be-119">Для этого требуется линейное понимание контроллера домена.</span><span class="sxs-lookup"><span data-stu-id="cb2be-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="cb2be-120">Объект Device, имеющий сертификат, синхронизируется с Azure AD через Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="cb2be-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="cb2be-121">По умолчанию цикл синхронизации выполняется каждые 30 минут, но зависит от конфигурации Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="cb2be-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="cb2be-122">Для получения дополнительных сведений обратитесь к этому [документу](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="cb2be-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="cb2be-123">На этом этапе вы должны увидеть устройство темы в состоянии "ожидается" в разделе "колонка устройства" на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cb2be-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="cb2be-124">При следующем входе пользователя в Windows 10 регистрация будет завершена.</span><span class="sxs-lookup"><span data-stu-id="cb2be-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="cb2be-125">Если вы находитесь в сети VPN, а процесс входа в систему завершается с подключением домена, регистрацию можно инициировать вручную:</span><span class="sxs-lookup"><span data-stu-id="cb2be-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="cb2be-126">Выдача дсрегкмд/Жоин локально в приглашении администратора или удаленно через PSExec для компьютера.</span><span class="sxs-lookup"><span data-stu-id="cb2be-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="cb2be-127">Например, PsExec – s \\ win10client01 cmd, дсрегкмд/Жоин</span><span class="sxs-lookup"><span data-stu-id="cb2be-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="cb2be-128">Дополнительные сведения об устранении проблем с гибридным присоединением приведены в [статье Устранение неполадок устройств](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="cb2be-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>

---
title: Условный доступ блокирует меня при использовании устройства, присоединенного к домену
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965471"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="0af32-102">Условный доступ блокирует меня при использовании устройства, присоединенного к домену</span><span class="sxs-lookup"><span data-stu-id="0af32-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="0af32-103">**Настоятельно рекомендуемые инструменты**</span><span class="sxs-lookup"><span data-stu-id="0af32-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="0af32-104">[Средство устранения неполадок с регистрацией устройств](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) — средство, помогающее устранять наиболее распространенные проблемы с регистрацией устройств.</span><span class="sxs-lookup"><span data-stu-id="0af32-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="0af32-105">[Сценарий тестирования подключения регистрации устройств](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) — сценарий, обеспечивающий доступ устройства к конечным точкам регистрации устройств в системной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0af32-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="0af32-106">[Сценарий очистки устройств Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) — сценарий, позволяющий искать устаревшие устройства в среде и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="0af32-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="0af32-107">Вот некоторые распространенные причины, по которым условный доступ не удается использовать для устройства, присоединенного к домену (гибридное присоединение к Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0af32-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="0af32-108">**На устройстве нет основного маркера обновления Azure AD**. На устройстве должен содержаться основной маркер обновления (PRT) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0af32-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="0af32-109">Дополнительные сведения о PRT см. в [этом документе](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="0af32-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="0af32-110">Чтобы проверить наличие основного маркера обновления Azure AD, можно выполнить команду `dsregcmd/status` на устройстве и убедиться, что параметру AzureAdPrt соответствует значение "ДА".</span><span class="sxs-lookup"><span data-stu-id="0af32-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="0af32-111">Если параметру AzureAdPrt соответствует значение "НЕТ", проверьте следующее.</span><span class="sxs-lookup"><span data-stu-id="0af32-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="0af32-112">**Используется ли федеративная среда с AD FS и доступна ли она из домашних сетей пользователей**. В этом случае убедитесь, что конечные точки usernamemixed доступны из экстрасети.</span><span class="sxs-lookup"><span data-stu-id="0af32-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="0af32-113">Если AD FS находится за VPN, пользователи должны подключиться к VPN и повторно войти в устройство.</span><span class="sxs-lookup"><span data-stu-id="0af32-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="0af32-114">Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="0af32-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="0af32-115">**Является ли доверенный платформенный модуль устройства неисправным (что не позволяет проверить подлинность устройства)**. Проверьте документ tpm.msc, чтобы узнать, находится ли доверенный платформенный модуль в состоянии "Готов".</span><span class="sxs-lookup"><span data-stu-id="0af32-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="0af32-116">В противном случае выполните команду `dsregcmd/leave` и позвольте устройству повторно присоединиться к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0af32-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="0af32-117">После этого повторите попытку.</span><span class="sxs-lookup"><span data-stu-id="0af32-117">Then, try again.</span></span> <span data-ttu-id="0af32-118">Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="0af32-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="0af32-119">**Используется сторонний поставщик удостоверений, не поддерживающий протокол WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="0af32-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="0af32-120">Как описано в наших документах, в этом случае устройства с гибридным присоединением к Azure AD не могут работать.</span><span class="sxs-lookup"><span data-stu-id="0af32-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="0af32-121">Обратитесь за поддержкой к своему поставщику удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0af32-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="0af32-122">**Пользователи используют браузер Chrome без учетных записей Windows 10** или **расширение Office для Chrome не использует автоматически PRT на устройствах, присоединенных к AAD, или с гибридным присоединением к AAD**. Это приводит к сбою политик условного доступа на основе устройств с отображением сообщения об ошибке "Незарегистрированное устройство".</span><span class="sxs-lookup"><span data-stu-id="0af32-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="0af32-123">Чтобы правильно использовать браузер Chrome, установите "Учетные записи Windows 10" или "Расширение Office для браузера Chrome пользователей" с помощью SCCM или Intune.</span><span class="sxs-lookup"><span data-stu-id="0af32-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="0af32-124">Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="0af32-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="0af32-125">Если невозможно удаленно установить расширение, уведомьте пользователей о необходимости установить одно из вышеперечисленных расширений вручную, чтобы получить доступ к приложениям, использующим условный доступ на основе устройств.</span><span class="sxs-lookup"><span data-stu-id="0af32-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="0af32-126">Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="0af32-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="0af32-127">**Устройство было правильно гибридно присоединено к Azure AD, но случайно удалено или отключено из-за изменений синхронизации в Azure AD Connect или с портала Azure**. В этом случае объект устройства больше не распознается как полностью присоединенное устройство, даже если для него отображается действительное состояние AzureAdJoined и PRT.</span><span class="sxs-lookup"><span data-stu-id="0af32-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="0af32-128">Чтобы устранить эту проблему, выполните команду `dsregcmd/leave` на затронутых устройствах и позвольте им повторно присоединиться к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0af32-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="0af32-129">Дополнительные сведения см. в [этом документе](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="0af32-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="0af32-130">Если ваши устройства работают под управлением Windows 10 с обновлением 1809 и VPN или облачным прокси-сервером и у вас возникают проблемы с состоянием AzureAdPrt или любая проблема приложения с единым входом (Outlook не подключается к почтовому ящику, даже если у вас был PRT), воспользуйтесь исправлением [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) или накопительным пакетом обновления [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) за апрель, чтобы предотвратить сбои PRT на этих компьютерах.</span><span class="sxs-lookup"><span data-stu-id="0af32-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>


















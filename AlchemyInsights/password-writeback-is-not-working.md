---
title: Не работает переописка пароля
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232784"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="1536c-102">Не работает переописка пароля</span><span class="sxs-lookup"><span data-stu-id="1536c-102">Password Writeback is not working</span></span>

<span data-ttu-id="1536c-103">**У меня возникают проблемы с настройкой перео записи паролей**</span><span class="sxs-lookup"><span data-stu-id="1536c-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="1536c-104">Функция записи паролей является важной функцией.</span><span class="sxs-lookup"><span data-stu-id="1536c-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="1536c-105">Убедитесь, что вы понимаете требования к лицензированию:</span><span class="sxs-lookup"><span data-stu-id="1536c-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="1536c-106">В вашей организации должна быть хотя бы одна лицензия</span><span class="sxs-lookup"><span data-stu-id="1536c-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="1536c-107">**Только облачные пользователи** : любой платный SKU Office 365 (O365) или Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="1536c-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="1536c-108">**Облачные и/или** локально пользователи — Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="1536c-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="1536c-109">Дополнительные информацию о требованиях к лицензированию см. в подраздиниях о требованиях лицензирования для самостоятельного сброса [паролей Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="1536c-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="1536c-110">У вас есть хотя бы одна учетная запись администратора и одна тестовая учетная запись пользователя с одной из соответствующих лицензий.</span><span class="sxs-lookup"><span data-stu-id="1536c-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="1536c-111">Для работы с записью пароля необходимо подключить Azure AD Connect к эмулятору основного контроллера домена.</span><span class="sxs-lookup"><span data-stu-id="1536c-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="1536c-112">Вы можете настроить Azure AD Connect для использования основного  контроллера домена, щелкнув правой кнопкой мыши свойства соединителя синхронизации Active Directory и выбрав разделы **каталогов.**</span><span class="sxs-lookup"><span data-stu-id="1536c-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="1536c-113">После этого найди **раздел** параметров подключения контроллера домена и поимейте, что в поле с заголовком "Использовать только предпочтительные **контроллеры домена".**</span><span class="sxs-lookup"><span data-stu-id="1536c-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="1536c-114">Если предпочтительный dc не является эмулятором PDC, Azure AD Connect по-прежнему будет связываться с PDC для записи пароля.</span><span class="sxs-lookup"><span data-stu-id="1536c-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="1536c-115">Сброс пароля настроен и включен в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1536c-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="1536c-116">Дополнительные сведения см. в подстановлении пользователями [паролей Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="1536c-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="1536c-117">Убедитесь, что учетная запись администратора, используемая для обеспечения записи пароля, является учетной записью администратора облака (созданная в Azure AD, а не локальной службе AD)</span><span class="sxs-lookup"><span data-stu-id="1536c-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="1536c-118">У вас есть локальное развертывание AD с одним или несколькими лесами под управлением Windows Server 2008 R2, Windows Server 2012 или Windows Server 2012 R2 с последними пакетами обновления</span><span class="sxs-lookup"><span data-stu-id="1536c-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="1536c-119">У вас установлено средство Azure AD Connect и вы подготовили среду AD для синхронизации с облаком.</span><span class="sxs-lookup"><span data-stu-id="1536c-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="1536c-120">Перед тестированием записи пароля убедитесь, что сначала вы выполните полный импорт и полную синхронизацию из AD и Azure AD в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1536c-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="1536c-121">Дополнительные узнать, как сделать полную синхронизацию [и полный импорт в Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="1536c-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="1536c-122">**У меня возникла проблема с подключением для записи паролей**</span><span class="sxs-lookup"><span data-stu-id="1536c-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="1536c-123">Скачивание и включении последней версии [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="1536c-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="1536c-124">Конфигурация брандмауэра: средству Azure AD Connect (1.1.443 и выше) потребуется исходящие **HTTPS-доступ** к:</span><span class="sxs-lookup"><span data-stu-id="1536c-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="1536c-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1536c-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="1536c-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="1536c-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="1536c-127">Разрешить простаивающим подключениям сохраняться не менее 2-3 минут</span><span class="sxs-lookup"><span data-stu-id="1536c-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="1536c-128">**У меня по-прежнему возникают проблемы с переописаемой паролем**</span><span class="sxs-lookup"><span data-stu-id="1536c-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="1536c-129">Если у вас по-прежнему возникли трудности, попробуйте отключить и повторно включив службу записи паролей в средстве Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="1536c-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="1536c-130">Чтобы узнать больше, узнайте, как отключить и повторно включить возможность записи [паролей](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="1536c-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>

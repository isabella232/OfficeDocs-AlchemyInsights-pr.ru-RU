---
title: Центр администрирования Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670377"
---
# <a name="teams-admin-center"></a><span data-ttu-id="351b8-102">Центр администрирования Teams</span><span class="sxs-lookup"><span data-stu-id="351b8-102">Teams Admin Center</span></span>

<span data-ttu-id="351b8-103">Ознакомьтесь с управлением Teams с помощью [Центра администрирования Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="351b8-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="351b8-104">Если вам не удается получить доступ к Центру администрирования Teams, проверьте следующее:</span><span class="sxs-lookup"><span data-stu-id="351b8-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="351b8-105">Проверьте, что вы разрешили соответствующие [IP-адреса и URL-адреса Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всех устройствах периметра (в брандмауэре и т. д.) и в правилах брандмауэра на локальном компьютере.</span><span class="sxs-lookup"><span data-stu-id="351b8-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="351b8-106">Убедитесь, что данные входа, используемые для доступа к порталу администрирования Teams, соответствуют имени пользователя, указанному на [портале администрирования Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="351b8-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="351b8-107">Если пользователи не отображаются в Центре администрирования Teams, проверьте следующее:</span><span class="sxs-lookup"><span data-stu-id="351b8-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="351b8-108">Вы создали пользователей или назначили лицензии в течение последних 24 часов?</span><span class="sxs-lookup"><span data-stu-id="351b8-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="351b8-109">Подождите не менее 24 часов, прежде чем создавать запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="351b8-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="351b8-110">Убедитесь, что вам назначены соответствующие лицензии.</span><span class="sxs-lookup"><span data-stu-id="351b8-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="351b8-111">Если вы пользуетесь локальной службой Active Directory, убедитесь в том, что [значение msRTCSIP-PrimaryUserAddress или адреса SIP в поле ProxyAddresses в локальной службе Active Directory уникально и его формат соответствует ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** пользователя в [Центре администрирования Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="351b8-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="351b8-112">Если вы планируете использовать развертывание Skype для бизнеса Server и разместить пользователей как локально, так и в сети, следуйте инструкциям в разделе **"Настройка гибридной среды для Teams и Skype для бизнеса в Интернете"** на информационной панели Skype for Business Server и переместите пользователей в Интернет.</span><span class="sxs-lookup"><span data-stu-id="351b8-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>

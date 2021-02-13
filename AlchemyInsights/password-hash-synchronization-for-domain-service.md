---
title: Синхронизация хэша паролей для службы домена
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162941"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="5b698-102">Синхронизация хэша паролей для службы домена</span><span class="sxs-lookup"><span data-stu-id="5b698-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="5b698-103">**Если ваш экземпляр Azure AD DS предлагает вам включить синхронизацию хэша паролей**</span><span class="sxs-lookup"><span data-stu-id="5b698-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="5b698-104">Это сценарий, в котором вы запускаете гибридную среду с пользователями, выполняя синхронизацию из локальной среды доменных служб Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="5b698-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="5b698-105">Этот сценарий выполняется несмотря на синхронизацию хэша паролей из локальной службы AD DS с клиентом Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5b698-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="5b698-106">**Причина**</span><span class="sxs-lookup"><span data-stu-id="5b698-106">**Cause**</span></span>

<span data-ttu-id="5b698-107">Azure AD Connect по умолчанию не синхронизирует хэши паролей NTLM и Kerberos прежних версий, необходимые для Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="5b698-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="5b698-108">**Временное решение**</span><span class="sxs-lookup"><span data-stu-id="5b698-108">**Workaround**</span></span> 

<span data-ttu-id="5b698-109">Вам нужно настроить в Azure AD Connect синхронизацию хэшей паролей, необходимых для проверки подлинности NTLM и Kerberos.</span><span class="sxs-lookup"><span data-stu-id="5b698-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="5b698-110">После настройки Azure AD Connect во время локального события создания учетной записи или изменения пароля хэши паролей прежних версий также будут синхронизироваться с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5b698-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="5b698-111">Дополнительные сведения об этом и рекомендации по включению синхронизации паролей в гибридных средах Azure AD DS см. [здесь](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).</span><span class="sxs-lookup"><span data-stu-id="5b698-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>
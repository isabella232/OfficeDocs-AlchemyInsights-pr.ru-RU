---
title: Устранение неполадок синхронизации паролей
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924709"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="b6cf7-102">Устранение неполадок синхронизации паролей</span><span class="sxs-lookup"><span data-stu-id="b6cf7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="b6cf7-103">Для устранения неполадок, которых нет пароли синхронизации с Azure AD подключить версии 1.1.614.0 или более поздней версии:</span><span class="sxs-lookup"><span data-stu-id="b6cf7-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="b6cf7-104">Откройте новый сеанс Windows PowerShell на сервере Azure AD подключиться с параметром **Запуск от имени администратора** .</span><span class="sxs-lookup"><span data-stu-id="b6cf7-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="b6cf7-105">Запустите **командлет Set-ExecutionPolicy RemoteSigned** или **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="b6cf7-106">Запустите мастер подключения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="b6cf7-107">Перейдите к \*\* дополнительные задачи \*\* выберите параметр \*\* Устранение \*\* и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="b6cf7-108">На странице "Устранение неполадок" щелкните меню **запуска, чтобы начать устранение неполадок** в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="b6cf7-109">В главном меню выберите **Устранение неполадок синхронизации паролей**.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="b6cf7-110">В меню sub выберите **синхронизации паролей вообще не работает**.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="b6cf7-111">**Изучите результаты задачу по устранению неполадок**</span><span class="sxs-lookup"><span data-stu-id="b6cf7-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="b6cf7-112">Устранения неполадок задачи выполняются следующие проверки:</span><span class="sxs-lookup"><span data-stu-id="b6cf7-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="b6cf7-113">Проверяет, что для вашего клиента Azure AD включена функция синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="b6cf7-114">Проверяет, что сервер подключить Azure AD не входит в режим временных файлов.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="b6cf7-115">Для каждого существующего локального Active Directory соединителя (который соответствует существующего леса Active Directory):</span><span class="sxs-lookup"><span data-stu-id="b6cf7-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="b6cf7-116">Проверяет, что включен компонент синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="b6cf7-117">Поиск события пульса синхронизации паролей в журнале событий приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="b6cf7-118">Для каждого домена Active Directory в разделе локальный Соединитель Active Directory:</span><span class="sxs-lookup"><span data-stu-id="b6cf7-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="b6cf7-119">Проверяет доступность с Azure AD подключение сервера домена.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="b6cf7-120">Проверяет, что учетные записи доменных служб Active Directory (AD DS), используется локальный Соединитель Active Directory имеет правильное имя пользователя, пароль и разрешения, необходимые для синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="b6cf7-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="b6cf7-121">Дополнительные сведения об устранении проблем синхронизации паролей в разделе [Синхронизация паролей Устранение неполадок с синхронизацией подключить Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="b6cf7-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  


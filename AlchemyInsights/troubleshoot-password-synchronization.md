---
title: Устранение неполадок при синхронизации паролей
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767189"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d6d8f-102">Устранение неполадок при синхронизации паролей</span><span class="sxs-lookup"><span data-stu-id="d6d8f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d6d8f-103">Устранение неполадок, в которых не синхронизируются пароли с Azure AD Connect версии 1.1.614.0 или более поздней.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d6d8f-104">Откройте новый сеанс Windows PowerShell на сервере Azure AD Connect с параметром **Запуск от имени администратора** .</span><span class="sxs-lookup"><span data-stu-id="d6d8f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="d6d8f-105">Выполните командлет **Set — ExecutionPolicy RemoteSigned** или **Set/ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="d6d8f-106">Запустите мастер Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="d6d8f-107">Перейдите на страницу \* \* дополнительные задачи \* \*, выберите \* \* Устранение неполадок \* \* и нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="d6d8f-108">На странице Устранение неполадок нажмите кнопку **запустить, чтобы запустить меню устранение неполадок** в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="d6d8f-109">В главном меню выберите пункт **устраненИе неполадок синхронизации паролей**.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="d6d8f-110">Во вложенном меню выберите пункт **Синхронизация паролей не работает**.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="d6d8f-111">**Общие сведения о результатах задачи "Устранение неполадок"**</span><span class="sxs-lookup"><span data-stu-id="d6d8f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d6d8f-112">Задача по устранению неполадок выполняет следующие проверки:</span><span class="sxs-lookup"><span data-stu-id="d6d8f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d6d8f-113">Проверка включения функции синхронизации паролей для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="d6d8f-114">Проверяет, находится ли сервер Azure AD Connect в режиме промежуточного хранения.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="d6d8f-115">Для каждого существующего локального соединителя Active Directory (соответствующего существующему лесу Active Directory):</span><span class="sxs-lookup"><span data-stu-id="d6d8f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="d6d8f-116">Проверяет, включена или отключена функция синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="d6d8f-117">Выполняет поиск событий пульса синхронизации паролей в журналах событий приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="d6d8f-118">Для каждого домена Active Directory в локальном соединителе Active Directory:</span><span class="sxs-lookup"><span data-stu-id="d6d8f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="d6d8f-119">Проверяет, достижим ли домен с сервера Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="d6d8f-120">Проверка того, что учетные записи доменных служб Active Directory (AD DS), используемые локальным соединителем Active Directory, имеют правильные имя пользователя, пароль и разрешения, необходимые для синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="d6d8f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="d6d8f-121">Дополнительные сведения об устранении неполадок при синхронизации паролей приведены [в разделе устраненИе неполадок с синхронизацией паролей с помощью Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d6d8f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  


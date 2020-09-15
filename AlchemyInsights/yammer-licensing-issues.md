---
title: Проблемы с лицензированием Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657289"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="9cc79-102">Проблемы с лицензированием Yammer</span><span class="sxs-lookup"><span data-stu-id="9cc79-102">Yammer licensing issues</span></span>

<span data-ttu-id="9cc79-103">У всех пользователей должна быть лицензия для применения службы Yammer корпоративный, но по умолчанию Yammer не требует наличия лицензии на доступ к службе.</span><span class="sxs-lookup"><span data-stu-id="9cc79-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="9cc79-104">Если администратор изменит этот параметр, чтобы заблокировать пользователей Microsoft 365 без лицензии Yammer, пользователи, которым не назначена лицензия Yammer корпоративный, не смогут получить доступ к службе Yammer.</span><span class="sxs-lookup"><span data-stu-id="9cc79-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="9cc79-105">Дополнительные сведения см. в статье [Управление лицензиями пользователей Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9cc79-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="9cc79-106">При удалении лицензий пользователей плитка Yammer больше не отображается, а другие службы могут скрыть функции путем удаления лицензии.</span><span class="sxs-lookup"><span data-stu-id="9cc79-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="9cc79-107">В других случаях функции могут по-прежнему отображаться, но для работы потребуется назначить лицензию.</span><span class="sxs-lookup"><span data-stu-id="9cc79-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="9cc79-108">**Лицензия для пользователя не обновляется**</span><span class="sxs-lookup"><span data-stu-id="9cc79-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="9cc79-109">Иногда пользователь, которому назначена лицензия, не может получить доступ к Yammer.</span><span class="sxs-lookup"><span data-stu-id="9cc79-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="9cc79-110">Чаще всего задержки возникают в процессе массового назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="9cc79-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="9cc79-111">Обновление пользователей Yammer может происходить не в том же порядке, в котором меняются лицензии в Azure AD, так как система работает асинхронно.</span><span class="sxs-lookup"><span data-stu-id="9cc79-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="9cc79-112">Подождите до 24 часов, прежде чем сообщать в службу поддержки о проблемах с синхронизацией лицензий.</span><span class="sxs-lookup"><span data-stu-id="9cc79-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="9cc79-113">**Массовое назначение лицензий**</span><span class="sxs-lookup"><span data-stu-id="9cc79-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="9cc79-114">Лицензии можно назначать через центр администрирования или сценарии PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9cc79-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="9cc79-115">Дополнительные сведения см. в статьях [Назначение лицензий пользователям](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и [Назначение лицензий для учетных записей пользователей с помощью PowerShell в Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="9cc79-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="9cc79-116">Служба поддержки Майкрософт не предоставляет помощь в создании сценариев, но документация по назначению лицензий Yammer доступна.</span><span class="sxs-lookup"><span data-stu-id="9cc79-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="9cc79-117">Дополнительные сведения см. в статье [Управление лицензиями Yammer с помощью Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="9cc79-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>
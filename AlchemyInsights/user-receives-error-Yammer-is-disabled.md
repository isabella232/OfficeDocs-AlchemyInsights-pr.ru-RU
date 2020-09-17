---
title: Пользователь получил сообщение об ошибке AADSTS7000112 "Yammer отключен"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796661"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="38daa-102">Пользователь получил сообщение об ошибке AADSTS7000112 "Yammer отключен"</span><span class="sxs-lookup"><span data-stu-id="38daa-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="38daa-103">Если появляется сообщение об ошибке "AADSTS7000112: Приложение '00000005-0000-0ff1-ce00-000000000000'(Yammer) отключено", это значит, что в субъекте-службе внутри Azure AD возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="38daa-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="38daa-104">Администратор мог отключить субъект-службу, чтобы заблокировать доступ к Yammer.</span><span class="sxs-lookup"><span data-stu-id="38daa-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="38daa-105">Отключение субъекта-службы не рекомендуется, это может привести к возникновению дополнительных проблем.</span><span class="sxs-lookup"><span data-stu-id="38daa-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="38daa-106">Подробнее о поддерживаемых способах блокирования доступа пользователей к Yammer см. в статье [Отключение доступа к Yammer для пользователей Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="38daa-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="38daa-107">Чтобы устранить эту ошибку на портале Azure и восстановить доступ пользователей к Yammer, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="38daa-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="38daa-108">Откройте страницу Azure Active Directory и на панели навигации слева выберите **Корпоративные приложения** из раздела **Управление**.</span><span class="sxs-lookup"><span data-stu-id="38daa-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="38daa-109">В поле поиска введите **Office 365 Yammer** и выберите имя приложения, чтобы открыть параметры.</span><span class="sxs-lookup"><span data-stu-id="38daa-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="38daa-110">Нажмите кнопку **Свойства** в разделе **Управление** на панели навигации слева.</span><span class="sxs-lookup"><span data-stu-id="38daa-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="38daa-111">Установите для параметра **Разрешать вход пользователям?** значение **Да**, а затем нажмите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="38daa-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="38daa-112">Повторно войдите в Yammer</span><span class="sxs-lookup"><span data-stu-id="38daa-112">Sign in to Yammer again.</span></span> <span data-ttu-id="38daa-113">Вам может понадобиться удалить файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="38daa-113">You might need to clear cookies.</span></span>

<span data-ttu-id="38daa-114">Вместо этого для установки значения можно выполнить команду PowerShell.</span><span class="sxs-lookup"><span data-stu-id="38daa-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="38daa-115">Подробнее см. в статье [Ошибка "При выполнении входа возникла проблема" при нажатии на плитку Yammer в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="38daa-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 
---
title: Устранение неполадок при синхронизации паролей
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387890"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="25856-102">Устранение неполадок при синхронизации паролей</span><span class="sxs-lookup"><span data-stu-id="25856-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="25856-103">Чтобы устранить проблемы с синхронизацией паролей, начните с использования этой задачи по устранению неполадок подключения AAD, чтобы определить причину, по которой не синхронизируются пароли.</span><span class="sxs-lookup"><span data-stu-id="25856-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="25856-104">Чтобы начать, перейдите к разделу [Управление прямой синхронизацией](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="25856-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="25856-105">Откройте новый сеанс Windows PowerShell на сервере Azure AD Connect и выберите пункт **Запуск от имени администратора** .</span><span class="sxs-lookup"><span data-stu-id="25856-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="25856-106">Выполните командлет Set — ExecutionPolicy RemoteSigned или Set/ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="25856-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="25856-107">Запустите мастер Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="25856-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="25856-108">Перейдите на страницу дополнительные задачи > " **Устранение неполадок**"  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="25856-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="25856-109">Нажмите кнопку **запустить** , чтобы открыть меню устранение неполадок PowerShell.</span><span class="sxs-lookup"><span data-stu-id="25856-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="25856-110">Выберите пункт **Устранение неполадок при синхронизации паролей**.</span><span class="sxs-lookup"><span data-stu-id="25856-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="25856-111">Эта ошибка обычно заключается в том, что пароль не синхронизируется для конкретной учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="25856-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="25856-112">**Примечания** Если время последней успешной синхронизации пароля прошло некоторое время, синхронизация паролей завершается с ошибкой назад.</span><span class="sxs-lookup"><span data-stu-id="25856-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="25856-113">Дополнительные сведения об устранении неполадок при синхронизации паролей приведены [в статье Устранение неполадок синхронизации паролей с помощью Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="25856-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>
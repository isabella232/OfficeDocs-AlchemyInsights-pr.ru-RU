---
title: Active Directory, не синхронизируются
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930988"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="29213-102">Active Directory, не синхронизируются</span><span class="sxs-lookup"><span data-stu-id="29213-102">Active Directory not syncing</span></span>

<span data-ttu-id="29213-103">Если вы получаете ошибки синхронизации, такие как "не последняя синхронизация", или обратите внимание на состояние синхронизации каталогов на портале администрирования Office: "Последняя синхронизация более 3 дней назад", возможно, AADConnect имеет неправильные параметры или недостаточно разрешений для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="29213-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="29213-104">Переустановка AADConnect с помощью экспресс-параметров может быстро устранить проблему:</span><span class="sxs-lookup"><span data-stu-id="29213-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="29213-105">[Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="29213-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="29213-106">[Следуйте инструкциям по экспресс-установке.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="29213-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="29213-107">Azure AD Connect необходимо устанавливать в операционной системе Windows Server 2012 или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="29213-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="29213-108">Этот сервер должен быть присоединен к домену, это может быть как контроллер домена, так и рядовой сервер.</span><span class="sxs-lookup"><span data-stu-id="29213-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="29213-109">Полный список требований и предварительных требований Azure AD Подключение просмотреть необходимые условия для [Azure AD Подключение.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="29213-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="29213-110">Дополнительные сведения об учетных записях службы AADConnect см. в статье [Azure AD Connect: учетные записи и разрешения](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="29213-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>

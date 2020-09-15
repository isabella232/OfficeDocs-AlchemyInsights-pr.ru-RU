---
title: Удаление потерянного пользователя из локального сервера
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680148"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="3d8c6-102">Удаление потерянного пользователя из локального сервера</span><span class="sxs-lookup"><span data-stu-id="3d8c6-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="3d8c6-103">Чтобы удалить потерянного пользователя, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="3d8c6-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="3d8c6-104">Выполните принудительную синхронизацию службы каталогов, следуя инструкциям в статье [Что такое гибридное удостоверение в Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="3d8c6-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="3d8c6-105">Для подтверждения синхронизации каталогов следуйте инструкциям в статье [Что такое гибридное удостоверение в Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="3d8c6-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="3d8c6-106">Если функция синхронизации работает должным образом, но удаление объекта Active Directory не переносится в Azure AD, необходимо вручную удалить потерянный объект с помощью одного из следующих командлетов Azure Active Directory для Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3d8c6-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="3d8c6-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="3d8c6-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="3d8c6-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="3d8c6-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="3d8c6-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="3d8c6-109">Remove-MsolUser</span></span>

    <span data-ttu-id="3d8c6-110">Например, чтобы удалить потерянный идентификатор пользователя john.smith@contoso.com, созданный с помощью синхронизации службы каталогов, запустите командлет.</span><span class="sxs-lookup"><span data-stu-id="3d8c6-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="3d8c6-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="3d8c6-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>
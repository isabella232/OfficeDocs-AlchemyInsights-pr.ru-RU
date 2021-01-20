---
title: Проблема с подключением к виртуальным машинам
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884615"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="7ec99-102">Проблема с подключением к виртуальным машинам</span><span class="sxs-lookup"><span data-stu-id="7ec99-102">Issue joining VMs</span></span>

<span data-ttu-id="7ec99-103">Чтобы устранить проблему, связанную с подключением к виртуальным машинам, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="7ec99-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="7ec99-104">Попробуйте войти в систему, используя формат **UPN** (например, 'joeuser@contoso.com') вместо формата **SAMAccountName** ('CONTOSO\joeuser').</span><span class="sxs-lookup"><span data-stu-id="7ec99-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="7ec99-105">Убедитесь, что синхронизация паролей включена в соответствии с инструкциями, описанными в *Руководстве по началу работы*.</span><span class="sxs-lookup"><span data-stu-id="7ec99-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="7ec99-106">Убедитесь, что затронутая учетная запись пользователя не является внешней учетной записью в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ec99-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="7ec99-107">Внешние пользователи не могут войти в управляемый домен, так как доменные службы Azure AD не имеют учетных данных для таких учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7ec99-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="7ec99-108">Если затронутая учетная запись пользователя является облачной учетной записью, убедитесь, что пользователи изменили свои пароли после включения доменных служб Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ec99-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="7ec99-109">Это действие приводит к созданию хэшей учетных данных, необходимых для доменных служб Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ec99-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="7ec99-110">Если затронутые учетные записи пользователей синхронизируются из локального каталога, убедитесь, что для выполнения полной синхронизации настроен рекомендуемый выпуск Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7ec99-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="7ec99-111">Если проблема сохраняется после выполнения Действия 4, выполните следующие команды с вашего устройства синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7ec99-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="7ec99-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="7ec99-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>
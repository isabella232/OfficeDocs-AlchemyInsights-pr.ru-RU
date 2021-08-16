---
title: Удаление или восстановление приложений
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102584"
---
# <a name="delete-or-restore-applications"></a>Удаление или восстановление приложений

**Удаление приложения из клиента Azure AD:**

1. На **портале Azure AD** выберите **Enterprise приложения.** Затем найдите и выберите приложение, которое необходимо удалить.
2. В разделе **Управление** в левой области выберите **Свойства**.
3. Выберите **Удаление,** а затем выберите **Да,** чтобы подтвердить, что вы хотите удалить приложение из клиента Azure AD.

Дополнительные сведения об удалении приложения см. в публикации [Quickstart: Delete an application from your Azure Active Directory Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

В PowerShell, в cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) удаляет конфигурации прокси-приложения из определенного приложения в Azure Active Directory и может удалить приложение полностью, если указано.

Вы можете **восстановить удаленное приложение с** помощью PowerShell. После идентифицированного приложения, которое необходимо восстановить, его можно восстановить с помощью [Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)

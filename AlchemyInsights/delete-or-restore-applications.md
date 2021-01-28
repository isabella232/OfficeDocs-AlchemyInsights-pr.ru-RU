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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013984"
---
# <a name="delete-or-restore-applications"></a>Удаление и восстановление приложений

**Чтобы удалить приложение из клиента Azure AD:**

1. На **портале Azure AD выберите** **корпоративные приложения.** Затем найдите и выберите приложение, которое нужно удалить.
2. В разделе **"Управление"** на левой области выберите **"Свойства".**
3. Выберите "Удалить", а затем выберите **"Да",** чтобы подтвердить удаление приложения из клиента Azure AD.

Дополнительные сведения об удалении приложения см. в кратком примере: удаление приложения из клиента [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

В PowerShell с использованием cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) удаляются конфигурации прокси приложения из определенного приложения в Azure Active Directory, и приложение можно полностью удалить, если указано.

Удаленное **приложение можно восстановить с помощью** PowerShell. После того как приложение, которое нужно восстановить, будет определено, его можно восстановить с помощью [Restore-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)

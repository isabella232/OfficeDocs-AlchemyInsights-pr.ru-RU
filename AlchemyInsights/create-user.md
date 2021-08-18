---
title: Создание пользователя
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323299"
---
# <a name="create-user"></a>Создание пользователя

**ОБЪЯВЛЕНИЕ:**

- [Обесценение поддержки регистрации WebView от Google с 4 января 2021 г.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Проверьте, могут ли приложения оказаться затронутыми, следуя указаниям [Google](https://go.microsoft.com/fwlink/?linkid=2157323) по тестированию совместимости.
- Убедитесь, что при входе в учетные записи Google пользователи используют веб-просмотр системы или системный браузер. Дополнительные сведения см. в статье [Проблемы при входе в приложения с помощью браузера Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Не удается создать нового пользователя в каталоге Azure AD**

1. Убедитесь, что у вас есть разрешение на создание нового стандартного пользователя. Только роль глобального администратора или администратора пользователя в Azure Active Directory (AD) может создать нового стандартного пользователя. Если у вас нет одной из этих ролей, попросите администратора назначить вам одну из этих ролей или создать для вас новую учетную запись пользователя.
1. Убедитесь, что имя пользователя находится в домене, проверенном в Azure AD. Если в Azure AD нет проверенных имен личного домена, вы можете использовать исходный домен Azure AD, заканчивающийся на *.onmicrosoft.com.
1. Убедитесь, что имя пользователя находится в домене, который не включен в федерацию Azure AD из локальной среды Active Directory. Пользователи с доменными именами, включенными в федерацию из локальной среды, не могут быть добавлены в облако.
1. Убедитесь, что другие пользователи или контакты не используют имя, которое необходимо назначить новому пользователю. Имена пользователей в Azure AD должны быть уникальными.
1. См. [роли и администраторы Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для вашей службы Azure AD.
1. См. [имена доменов](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для вашей службы Azure AD.
1. Чтобы получить подробные сведения о недавно созданном или удаленном пользователе, например о том, кто и когда выполнил это действие, проверьте [журналы аудита](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators).
1. Дополнительные сведения о добавлении новых пользователей см. в сайте Использование портала Azure для создания нового пользователя [в Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Административные роли Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)разрешения на роль администратора в Azure Active Directory
1. Вы также можете [использовать Azure AD PowerShell для создания нового пользователя.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)

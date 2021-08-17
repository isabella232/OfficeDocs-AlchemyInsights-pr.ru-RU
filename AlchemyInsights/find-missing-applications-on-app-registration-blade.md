---
title: Поиск отсутствующих приложений на лезвии регистрации приложений
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057115"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Поиск отсутствующих приложений на лезвии регистрации приложений

1. Не удается найти приложения на портале регистрации приложений.

    Если приложение является приложением с несколькими клиентами и оно было зарегистрировано в другом клиенте, оно не будет отображаться в лезвии регистрации приложений. Однако вы можете найти его в Enterprise приложениях после того, как он был доступ (после получения согласия) и директор службы был создан в вашем клиенте. Дополнительные сведения см. в [& в Azure AD — платформа удостоверений Майкрософт.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Не удается просматривать приложения в лезвии регистрации приложений, даже если вы администратор.

    Убедитесь, что вы находитесь в правильном каталоге на портале Azure.
3. Мое приложение не перечислены в Enterprise приложениях, но оно появляется при запросе команды PowerShell.

    Иногда после удаления приложения с портала Azure оно не показывается на портале, но может быть удалено не полностью. Дополнительные сведения см. в указанных ниже статьях.
    - Вы можете получить список ранее удаленных приложений и узнать, появляется ли приложение в списке с помощью команды Powershell: **Get-AzureADDeletedApplication.** Дополнительные дополнительные информации см. в [видеоролике Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Если вы хотите удалить приложение полностью, вы можете попробовать следующее в PowerShell: **Remove-AzureADApplication-ObjectId**. Дополнительные дополнительные информации см. в [см. врезки Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Кроме того, вы можете попытаться восстановить удаленное приложение с помощью следующей команды Powershell: **Восстановление AzureADDeletedApplication-ObjectId**. Дополнительные дополнительные дополнительные функции см. в см. в [видеоролике Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Не может найти список всех предварительно установленных корпоративных приложений в моем новом клиенте Azure.

    Предварительно установленных корпоративных приложений в Azure AD по умолчанию нет. Его необходимо добавлять вручную из параметра "Новое приложение", просматривая его в галерее Azure AD или добавляя приложение без галереи. Дополнительные дополнительные информации см. в [видеоролике Quickstart: Добавление](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)приложения в Azure Active Directory клиента Azure AD.
    Если вы глобальный администратор, вы можете легко получить доступ к приложениям с [помощью Microsoft 365 app Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Невозможно найти мои приложения на портале "Мои приложения".

    Убедитесь, что приложения не скрыты на странице коллекции "Мои приложения". Дополнительные новости см. [в выпуске Collections (preview) на портале My Apps - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Чтобы запустить приложения с портала "Мои приложения", см. в & на портале My [Apps - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Приложение Mover не отображается на Enterprise приложениях после установки.

    Приложение "Office 365 Mover" — это мультитенантное приложение, которое не нужно добавлять в AAD с помощью раздела Приложения Gallery в разделе Enterprise Регистрация приложений. Чтобы получить Office 365 Mover, просто впишитесь в приложение, и оно запросит согласие пользователя на разрешения. После того как пользователь предоставляет согласие, это приложение автоматически будет добавлено к клиенту с id электронной почты, в который вы вошли.

    После входа в приложение вы сможете найти запись этого приложения под Enterprise приложениями в AAD. Для поиска этого приложения необходимо либо ввести полное имя, то есть "Office 365 Mover", либо просто поискать "office", и оно должно перечислить приложение. Подробнее см. в [Office 365 Mover говорит,](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)что он уже установлен, но не указан в Enterprise application gallery.
8. [Quickstart.](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) Просмотр списка приложений, использующих клиента Azure Active Directory (Azure AD) для управления удостоверениями, показывает, как просматривать приложения, также известные как приложения, которые уже настроены для использования клиента Azure AD в качестве поставщика удостоверений (IdP).
9. [Устранение распространенных](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) проблем с добавлением или удалением приложения для Azure Active Directory помогает понять общие проблемы, с которыми сталкиваются люди, просматривающие приложения в Azure Active Directory.

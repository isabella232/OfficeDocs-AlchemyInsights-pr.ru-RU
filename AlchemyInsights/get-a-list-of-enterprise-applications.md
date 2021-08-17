---
title: Получение списка Enterprise приложений
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116741"
---
# <a name="get-a-list-of-enterprise-applications"></a>Получение списка Enterprise приложений

1. Чтобы **получить** список корпоративных приложений (все приложения или фильтруются по имени Display, идентификатору, ИДЕНТИФИКАТОРу идентификатора и т.д.) с помощью команды Powershell, см. в приложении [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Чтобы получить список основных объектов службы (все объекты или фильтруются по ID) с помощью команды Powershell, см. в обзоре [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Если вы хотите получить список приложений, настроенных samL, вам помогут следующие скрипты **PowerShell:**

    Каждое приложение, в том числе приложение OAuth или SAML (как галереи, так и приложения, не в галерее), будет иметь два объекта, созданных в AAD при их регистрации. Один из них называется объектом приложения, а другой — объектом Service Principal. При сбросе свойств основного объекта службы с помощью PowerShell вы найдете, что каждое приложение имеет определенное количество тегов, связанных с ним, как:

    - OAuth apps would have a tag called **"WindowsAzureActiveDirectoryIntegratedApp"**
    - Приложение SAML Gallery будет иметь тег **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**
    - Non-Gallery SAML Apps would have a tag called **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**

    Таким образом, вы можете использовать эти теги и узнать, что это такое приложение. Тег **"WindowsAzureActiveDirectoryIntegratedApp"** является общим для всех типов приложений. Вы можете использовать следующий фрагмент, чтобы перечислить все приложения SAML (как в галерее, так и в негалерее):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Дополнительные сведения см. в [видеоролике Определение приложений с поддержкой SAML в Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Поиск и список только** веб-приложений: Используйте приведенную ниже команду, чтобы получить все приложения Azure AD с типом приложения "Веб-приложение/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Найдите и перечислить** только приложения Native: запустите следующую команду, чтобы получить все приложения для родных клиентов (настольных компьютеров и мобильных устройств).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. Экспорт всех зарегистрированных сведений **о приложениях Azure AD в CSV:** ниже команда экспортирует все приложения Azure AD с требуемой подробными сведениями в csv-файл:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation-Encoding UTF8

7. **Необходимо экспортировать список неиспользованых приложений Azure** — отчет аудита

    Azure AD может показывать журналы приложений только в течение 30 дней при Azure AD Premium лицензии.
    У вас есть два варианта хранения данных дольше 30 дней. API отчетов [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) можно использовать для получения данных программным образом и хранения их в базе данных. Кроме того, можно интегрировать журналы аудита в сторонние системы SIEM.

    Вы также можете скачать список приложений для всех приложений и приложений в Azure Active directory>Регистрация приложений>Загрузка>Все приложения и собственные приложения.

    Чтобы получить список приложений с помощью ms Graph, см. в приложении List [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) и типе ресурсов приложений [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).

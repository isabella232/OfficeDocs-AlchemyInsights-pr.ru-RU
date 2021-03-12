---
title: Проблемы со ссылками и URL-адресами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707895"
---
# <a name="issues-with-links-and-urls"></a>Проблемы со ссылками и URL-адресами

URI перенаправления и URL-адреса ответа (оба выражения взаимозаменяемы) — это URL-адреса, используемые платформой удостоверений Майкрософт для возврата маркеров, запрашиваемых приложениями. Сведения об этих URL-адресах см. в следующих статьях:

- [Потоки проверки подлинности и сценарии приложений](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) — сведения об URI перенаправления на странице **Регистрация приложения** для каждого сценария.
- [Ограничения URI перенаправления/URL-адреса ответа](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Я не знаю, как зарегистрировать правильный URI перенаправления или URL-адрес ответа для своего приложения**

Если при входе в разрабатываемое приложение в диалоговом окне входа отображается сообщение **AADSTS50011: URL-адрес ответа, указанный в запросе, не совпадает с URL-адресами ответа, настроенными для приложения <your app ID>**, вам потребуется добавить в регистрацию приложения URI перенаправления, использованный вашим кодом в запросе маркера для платформы удостоверений Майкрософт.

Чтобы добавить URL-адрес ответа, перейдите на вкладку **Проверка подлинности** на странице **Регистрация приложения** на портале Azure и добавьте запись в разделе **URI перенаправления**. Значение, которое нужно ввести, зависит от типа создаваемого приложения, как описано ниже.

- Для одностраничных приложений и веб-приложений URL-адрес ответа является URL-адресом в вашем приложении. См. раздел [Регистрация одностраничного приложения](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) или [Регистрации веб-приложения с помощью портала Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Для классических приложений значение, которое требуется выбрать, зависит от:
    - платформы (MacOS отличается от Windows или Linux)
    - способа получения маркера (в интерактивном режиме, с помощью потока кода устройства, с помощью встроенной проверки подлинности Windows [IWA] или с именем пользователя и паролем).
    Дополнительные сведения см. в разделе [Классические приложения — регистрация приложения — URI перенаправления](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Для мобильных приложений URI перенаправления зависит от:
    - платформы (iOS/Android/UWP)
    - сведений, которые использовались для создания приложения, таких как идентификатор пакета в iOS, имя пакета и хэш подписи для Android. Эти сведения доступны в разделе регистрации приложения на портале Azure. Дополнительные сведения см. в разделе [Настройка платформы и URI перенаправления](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Веб-API и некоторые автоматические способы получения маркеров (IWA и имя пользователя/пароль) не требуют URI перенаправления.

**Я развернул веб-приложение, и при тестировании развернутого приложения выводится сообщение о несоответствии URL-адреса ответа**

Добавьте URI перенаправления для всех расположений, в которых вы разворачиваете свое веб-приложение. Дополнительные сведения см. в разделе [Регистрация веб-приложения с помощью портала Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Добавьте URI перенаправления для расположения сразу после развертывания приложения в этом расположении.

**Не удается зарегистрировать достаточное количество URL-адресов ответа**

Вы являетесь независимым поставщиком программного обеспечения, и у вас есть один или несколько URI перенаправления для каждого клиента. Вы хотите выполнить миграцию с ADAL/Azure AD версии 1.0 на MSAL/платформу удостоверений Майкрософт и достигли [максимального количества URI переадресации](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Чтобы устранить эту проблему, [добавьте URI перенаправления в субъекты-службы](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), соответствующие каждому клиенту.

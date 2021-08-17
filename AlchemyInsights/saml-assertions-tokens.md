---
title: SamL Assertions (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109253"
---
# <a name="saml-assertions-tokens"></a>SamL Assertions (Tokens)

1. Маркеры Языковой разметки утверждений безопасности являются XML-представлениями утверждений. По умолчанию маркеры SAML, Windows Средства связи (WCF), использующиеся в федеративных сценариях безопасности, выпускаются маркерами. Дополнительные сведения см. [в рублях SAML Tokens and Claims.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. В платформа удостоверений Майкрософт при обработке каждого потока проверки подлинности выделяется несколько типов маркеров безопасности. [Ссылка на утверждения маркера SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) описывает формат, характеристики безопасности и содержимое маркеров SAML 2.0.
3. Следуйте указаниям в настраиваемых сроках служб маркеров [в платформа удостоверений Майкрософт,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) чтобы понять, как настроить сроки служб маркеров.
4. Следуйте шагам, описанным в [этой статье,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) чтобы понять, как настроить шифрование маркеров Azure AD SAML.
5. В Azure AD можно настроить параметры подписи сертификатов и алгоритм подписи сертификатов. Дополнительные сведения см. в дополнительных параметрах подписи сертификатов в [маркере SAML для](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)приложений галереи в Azure Active Directory.

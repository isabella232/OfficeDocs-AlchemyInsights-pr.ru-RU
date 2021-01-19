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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884616"
---
# <a name="saml-assertions-tokens"></a>SamL Assertions (Tokens)

1. Маркеры SAML — это XML-представления утверждений. По умолчанию маркеры SAML, которые Windows Communication Foundation (WCF) использует в сценариях федеративной безопасности, являются маркерами выдачи. Дополнительные сведения [см. в подзаголовках маркеров и утверждений SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Платформа удостоверений Майкрософт выдает несколько типов маркеров безопасности при обработке каждого потока проверки подлинности. [Справочник по утверждениям маркеров SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) описывает формат, характеристики безопасности и содержимое маркеров SAML 2.0.
3. Следуйте указаниям в настройках времени существования маркера на платформе [удостоверений Майкрософт,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) чтобы понять, как настроить время жизни маркера.
4. Выполните действия, описанные в [этой статье,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) чтобы понять, как настроить шифрование маркеров SAML Azure AD.
5. В Azure AD можно настроить параметры подписи сертификатов и алгоритм подписи сертификатов. Дополнительные сведения см. в дополнительных параметрах [подписи сертификатов в маркере SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)для приложений коллекции в Azure Active Directory.

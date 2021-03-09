---
title: Устранение проблем, связанных с сертификатами подписи SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529276"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Устранение проблем, связанных с сертификатами подписи SAML

Чтобы устранить проблему с сертификатом подписи SAML, выполните следующие рекомендуемые действия.

1. При добавлении корпоративного приложения, поддерживающего единый вход, Azure создает сертификат, называемый [сертификатом подписи SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Срок действия этого сертификата составляет 3 года. Чтобы изменить дату окончания срока действия сертификата, см. раздел [Настройка даты окончания срока действия сертификата федерации и его замена новым сертификатом](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure будет использовать этот сертификат для подписи маркеров SAML, запрашиваемых приложением, и для отправки их приложению для успешного единого входа. Чтобы завершить эту процедуру, скачайте сертификат с портала Azure и отправьте его поставщику приложения для завершения процесса единого входа.

После завершения этого процесса ваше приложение будет доверять этому сертификату, и все маркеры SAML, подписанные этим сертификатом, будут приниматься приложением.

3. Если срок действия этого сертификата истек, создайте новый сертификат, обновите его у поставщика приложения и активируйте его на стороне Azure. Дополнительные сведения см. в разделе [Обновление сертификата с истекающим сроком действия](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Если срок действия сертификата истек, пользователь не будет заблокирован.

4. [Добавьте адрес электронной почты для уведомлений](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration), отправляемых до истечения срока действия текущего сертификата.

> [!NOTE]
> Этап 4 является необязательным.

5. Измените параметры подписи сертификата SAML приложения и алгоритм подписи сертификата. Дополнительные сведения см. в разделе [Изменение параметров подписи сертификата и алгоритма подписи](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).


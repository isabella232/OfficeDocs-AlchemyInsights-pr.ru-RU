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
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="5cf4d-102">Устранение проблем, связанных с сертификатами подписи SAML</span><span class="sxs-lookup"><span data-stu-id="5cf4d-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="5cf4d-103">Чтобы устранить проблему с сертификатом подписи SAML, выполните следующие рекомендуемые действия.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5cf4d-104">При добавлении корпоративного приложения, поддерживающего единый вход, Azure создает сертификат, называемый [сертификатом подписи SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="5cf4d-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="5cf4d-105">Срок действия этого сертификата составляет 3 года.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="5cf4d-106">Чтобы изменить дату окончания срока действия сертификата, см. раздел [Настройка даты окончания срока действия сертификата федерации и его замена новым сертификатом](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="5cf4d-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="5cf4d-107">Azure будет использовать этот сертификат для подписи маркеров SAML, запрашиваемых приложением, и для отправки их приложению для успешного единого входа.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="5cf4d-108">Чтобы завершить эту процедуру, скачайте сертификат с портала Azure и отправьте его поставщику приложения для завершения процесса единого входа.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="5cf4d-109">После завершения этого процесса ваше приложение будет доверять этому сертификату, и все маркеры SAML, подписанные этим сертификатом, будут приниматься приложением.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="5cf4d-110">Если срок действия этого сертификата истек, создайте новый сертификат, обновите его у поставщика приложения и активируйте его на стороне Azure.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="5cf4d-111">Дополнительные сведения см. в разделе [Обновление сертификата с истекающим сроком действия](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="5cf4d-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="5cf4d-112">Если срок действия сертификата истек, пользователь не будет заблокирован.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="5cf4d-113">[Добавьте адрес электронной почты для уведомлений](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration), отправляемых до истечения срока действия текущего сертификата.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="5cf4d-114">Этап 4 является необязательным.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="5cf4d-115">Измените параметры подписи сертификата SAML приложения и алгоритм подписи сертификата.</span><span class="sxs-lookup"><span data-stu-id="5cf4d-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="5cf4d-116">Дополнительные сведения см. в разделе [Изменение параметров подписи сертификата и алгоритма подписи](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="5cf4d-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>


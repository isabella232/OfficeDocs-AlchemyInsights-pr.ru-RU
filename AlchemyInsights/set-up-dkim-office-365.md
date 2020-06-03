---
title: Настройка DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509397"
---
# <a name="setup-dkim"></a><span data-ttu-id="66b4f-102">Настройка DKIM</span><span class="sxs-lookup"><span data-stu-id="66b4f-102">Setup DKIM</span></span>

<span data-ttu-id="66b4f-103">В [этой статье](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)приведены полные инструкции по настройке DKIM для пользовательских доменов в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="66b4f-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="66b4f-104">Для **каждого** настраиваемого домена необходимо создать **две** записи CNAME DKIM в службе хостинга DNS вашего домена (обычно это регистратор доменных имен).</span><span class="sxs-lookup"><span data-stu-id="66b4f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="66b4f-105">Например, contoso.com и fourthcoffee.com должны иметь четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="66b4f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="66b4f-106">Записи CNAME DKIM для **каждого** пользовательского домена используют следующие форматы:</span><span class="sxs-lookup"><span data-stu-id="66b4f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="66b4f-107">**Имя узла**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="66b4f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="66b4f-108">**Указывает на адрес или значение**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="66b4f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="66b4f-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="66b4f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="66b4f-110">**Имя узла**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="66b4f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="66b4f-111">**Указывает на адрес или значение**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="66b4f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="66b4f-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="66b4f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="66b4f-113">\<DomainGUID\>— Это текст, расположенный слева `.mail.protection.outlook.com` в настраиваемой записи MX для пользовательского домена (например, `contoso-com` для домена contoso.com).</span><span class="sxs-lookup"><span data-stu-id="66b4f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="66b4f-114">\<InitialDomain\>— Это домен, который вы использовали при регистрации в Microsoft 365 (например, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="66b4f-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="66b4f-115">Создав записи CNAME для пользовательских доменов, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="66b4f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="66b4f-116">a.</span><span class="sxs-lookup"><span data-stu-id="66b4f-116">a.</span></span> <span data-ttu-id="66b4f-117">[Войдите в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с помощью рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="66b4f-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="66b4f-118">b.</span><span class="sxs-lookup"><span data-stu-id="66b4f-118">b.</span></span> <span data-ttu-id="66b4f-119">В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.</span><span class="sxs-lookup"><span data-stu-id="66b4f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="66b4f-120">c.</span><span class="sxs-lookup"><span data-stu-id="66b4f-120">c.</span></span> <span data-ttu-id="66b4f-121">В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="66b4f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="66b4f-122">г.</span><span class="sxs-lookup"><span data-stu-id="66b4f-122">d.</span></span> <span data-ttu-id="66b4f-123">Перейдите в раздел **Защита**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="66b4f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="66b4f-124">д.</span><span class="sxs-lookup"><span data-stu-id="66b4f-124">e.</span></span> <span data-ttu-id="66b4f-125">Выберите домен, а затем выберите **включить** для **подписи сообщений для этого домена с DKIM подписями**.</span><span class="sxs-lookup"><span data-stu-id="66b4f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="66b4f-126">Повторите этот шаг для каждого личного домена.</span><span class="sxs-lookup"><span data-stu-id="66b4f-126">Repeat this step for each custom domain.</span></span>

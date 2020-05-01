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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645685"
---
# <a name="setup-dkim"></a><span data-ttu-id="7b533-102">Настройка DKIM</span><span class="sxs-lookup"><span data-stu-id="7b533-102">Setup DKIM</span></span>

<span data-ttu-id="7b533-103">В [этой статье](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)приведены полные инструкции по настройке DKIM для пользовательских доменов в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b533-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="7b533-104">Для **каждого** настраиваемого домена необходимо создать **две** записи CNAME DKIM в службе хостинга DNS вашего домена (обычно это регистратор доменных имен).</span><span class="sxs-lookup"><span data-stu-id="7b533-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="7b533-105">Например, contoso.com и fourthcoffee.com должны иметь четыре записи CNAME DKIM: две для contoso.com и две для fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="7b533-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="7b533-106">Записи CNAME DKIM для **каждого** пользовательского домена используют следующие форматы:</span><span class="sxs-lookup"><span data-stu-id="7b533-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="7b533-107">**Имя узла**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7b533-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7b533-108">**Указывает на адрес или значение**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7b533-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7b533-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7b533-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="7b533-110">**Имя узла**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7b533-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7b533-111">**Указывает на адрес или значение**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7b533-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7b533-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7b533-112">**TTL**: 3600</span></span>

   <span data-ttu-id="7b533-113">\<DomainGUID\> — текст слева от `.mail.protection.outlook.com` настраиваемой записи MX для пользовательского домена (например, `contoso-com` для домена contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7b533-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="7b533-114">\<Инитиалдомаин\> — это домен, который вы использовали при регистрации в Microsoft 365 (например, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="7b533-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="7b533-115">Создав записи CNAME для пользовательских доменов, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="7b533-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="7b533-116">а.</span><span class="sxs-lookup"><span data-stu-id="7b533-116">a.</span></span> <span data-ttu-id="7b533-117">[Войдите в Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) с помощью рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="7b533-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="7b533-118">б)</span><span class="sxs-lookup"><span data-stu-id="7b533-118">b.</span></span> <span data-ttu-id="7b533-119">В левом верхнем углу щелкните значок средства запуска приложений и выберите **Администратор**.</span><span class="sxs-lookup"><span data-stu-id="7b533-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="7b533-120">в.</span><span class="sxs-lookup"><span data-stu-id="7b533-120">c.</span></span> <span data-ttu-id="7b533-121">В области навигации слева внизу разверните узел **Администратор** и выберите элемент **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7b533-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="7b533-122">г.</span><span class="sxs-lookup"><span data-stu-id="7b533-122">d.</span></span> <span data-ttu-id="7b533-123">Перейдите в раздел **Защита** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="7b533-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="7b533-124">д.</span><span class="sxs-lookup"><span data-stu-id="7b533-124">e.</span></span> <span data-ttu-id="7b533-125">Выберите домен, а затем выберите **включить** для **подписи сообщений для этого домена с DKIM подписями**.</span><span class="sxs-lookup"><span data-stu-id="7b533-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="7b533-126">Повторите этот шаг для каждого личного домена.</span><span class="sxs-lookup"><span data-stu-id="7b533-126">Repeat this step for each custom domain.</span></span>

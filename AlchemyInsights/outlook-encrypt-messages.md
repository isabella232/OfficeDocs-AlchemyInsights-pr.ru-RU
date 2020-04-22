---
title: S/MIME в Outlook в Интернете
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764885"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="0470b-102">Шифрование сообщений электронной почты в Outlook</span><span class="sxs-lookup"><span data-stu-id="0470b-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="0470b-103">Microsoft 365 шифрование сообщений основано на Microsoft Azure Rights Management (Azure RMS), которая входит в Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="0470b-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="0470b-104">Если ваша подписка включает Azure Rights Management или Azure Information Protection, **вам не нужно выполнять какие – либо действия для включения или отключения** службы управления правами вручную.</span><span class="sxs-lookup"><span data-stu-id="0470b-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="0470b-105">В зависимости от отзывов клиентов мы больше не сможете включить правила для почтовых ящиков Exchange для автоматического шифрования исходящей электронной почты с определенным типом конфиденциальной информации в клиенте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0470b-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="0470b-106">Вместо этого мы предоставляем подробные инструкции по выполнению йоурселвес.</span><span class="sxs-lookup"><span data-stu-id="0470b-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="0470b-107">Дополнительные сведения о том, как создать правило транспорта для шифрования конфиденциальной информации, можно найти в [этой статье](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="0470b-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="0470b-108">При использовании Outlook в Интернете **(ранее Outlook Web App**): при создании сообщения электронной почты просто нажмите кнопку **Защита** в OWA.</span><span class="sxs-lookup"><span data-stu-id="0470b-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="0470b-109">Будет применено разрешение "не пересылать".</span><span class="sxs-lookup"><span data-stu-id="0470b-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="0470b-110">Нажмите кнопку **изменить разрешение** и выберите **Шифрование** только для шифрования сообщения.</span><span class="sxs-lookup"><span data-stu-id="0470b-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="0470b-111">Если используется **клиент Outlook**: для отправки зашифрованного сообщения из Outlook 2013 или 2016 или Outlook 2016 для Mac, выберите **Параметры** > **разрешения**, а затем выберите необходимый вариант защиты.</span><span class="sxs-lookup"><span data-stu-id="0470b-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="0470b-112">Чтобы **автоматически шифровать все сообщения** , отправленные определенным получателям или партнерским организациям, необходимо создать правило транспорта для поток обработки почты в центре администрирования Exchange.</span><span class="sxs-lookup"><span data-stu-id="0470b-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="0470b-113">Подробные инструкции приведены в [этой статье support](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="0470b-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>


---
title: S/MIME в Outlook в Интернете
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772311"
---
# <a name="encrypt-email-messages-in-outlook"></a>Шифрование сообщений электронной почты в Outlook

Microsoft 365 шифрование сообщений основано на Microsoft Azure Rights Management (Azure RMS), которая входит в Azure Information Protection. Если ваша подписка включает Azure Rights Management или Azure Information Protection, **вам не нужно выполнять какие – либо действия для включения или отключения** службы управления правами вручную.

В зависимости от отзывов клиентов мы больше не сможете включить правила для почтовых ящиков Exchange для автоматического шифрования исходящей электронной почты с определенным типом конфиденциальной информации в клиенте по умолчанию. Вместо этого мы предоставляем подробные инструкции по выполнению йоурселвес. Дополнительные сведения о том, как создать правило транспорта для шифрования конфиденциальной информации, можно найти в [этой статье](https://aka.ms/OmeEtr).

- При использовании Outlook в Интернете **(ранее Outlook Web App**): при создании сообщения электронной почты просто нажмите кнопку **Защита** в OWA. Будет применено разрешение "не пересылать". Нажмите кнопку **изменить разрешение** и выберите **Шифрование** только для шифрования сообщения.

- Если используется **клиент Outlook**: для отправки зашифрованного сообщения из Outlook 2013 или 2016 или Outlook 2016 для Mac, выберите **Параметры**  >  **разрешения**, а затем выберите необходимый вариант защиты.

- Чтобы **автоматически шифровать все сообщения** , отправленные определенным получателям или партнерским организациям, необходимо создать правило транспорта для поток обработки почты в центре администрирования Exchange. Подробные инструкции приведены в [этой статье support](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).


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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010737"
---
# <a name="encrypt-email-messages-in-outlook"></a>Шифрование сообщений электронной почты в Outlook

Microsoft 365 Шифрование сообщений построено на Microsoft Azure управления правами (Azure RMS), который является частью Azure Information Protection. Если ваша подписка включает управление правами Azure или Azure Information Protection, вам не нужно принимать никаких действий, чтобы вручную включить или **активировать** службу управления правами.

Исходя из отзывов клиентов, мы больше не будем Exchange правила потока почты автоматически шифровать исходящую электронную почту, содержащую определенный тип конфиденциальной информации в клиенте по умолчанию. Вместо этого мы предоставляем подробные инструкции о том, как вы можете сделать это самостоятельно. Дополнительные сведения о создании правила транспорта для шифрования конфиденциальной информации см. [в этой статье.](https://aka.ms/OmeEtr)

- При использовании Outlook в Интернете (ранее **OWA):** При составления сообщения электронной почты просто нажмите **кнопку Защитить** в OWA. Это будет применяться разрешение "Не переададовать". Нажмите **кнопку Изменение разрешения** и выберите **Шифровать** только для шифрования сообщения.

- При использовании **Outlook** клиента: чтобы отправить зашифрованное сообщение от Outlook 2013 или 2016 г. или Outlook 2016 для Mac, выберите **параметры**  >  **Permissions,** а затем выберите необходимый параметр защиты.

- Чтобы **автоматически шифровать** всю электронную почту, отправленную определенным получателям или внешним организациям-партнерам, необходимо создать правило транспорта потока почты в центре администрирования Exchange. Подробные инструкции предоставляются в [этой статье поддержки](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).


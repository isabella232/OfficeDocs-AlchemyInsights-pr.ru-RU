---
title: 726 блокировка переадресации электронной почты
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478334"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Блокировка или разблокировка переадресации электронной почты

Чтобы включить или отключить переадресацию электронной почты для определенного почтового ящика, ознакомьтесь со статьей [Настройка переадресации электронной почты](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

На уровне клиента управление внешней пересылкой выполняется с помощью политики исходящей нежелательной почты. Вы можете проверить политику фильтрации исходящих сообщений в центре безопасности и соответствия требованиям [здесь](https://protection.office.com/antispam) или с помощью [команды Get – хостедаутбаундспамфилтерполици](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Если вы получаете следующее сообщение об ошибке: **"550 5.7.520 отказано в доступе, ваша организация не поддерживает внешнюю переадресацию**, убедитесь, что она настроена на включение внешнего автоматического перенаправления.

**Примечание:** Рекомендуется оставить внешнюю пересылку отключенной в политике фильтрации нежелательной почты по умолчанию и включить ее только для тех пользователей, которым требуется внешняя переадресация, создав пользовательскую политику для этих пользователей. Дополнительные сведения можно узнать в статье [Настройка переадресации внешних сообщений электронной почты в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
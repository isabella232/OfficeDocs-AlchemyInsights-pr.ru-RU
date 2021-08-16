---
title: Политики хранения в центре администрирования Exchange не работают
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074945"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Политики хранения в Exchange Центре администрирования

Если вы хотите, чтобы мы запускали автоматические проверки указанных ниже параметров, выберите кнопку < -- в верхней части этой страницы, а затем введите адрес электронной почты пользователя, у которого возникли проблемы с политиками хранения.

Если у вас возникли проблемы с политиками хранения в центре администрирования Exchange, которые не применяются к почтовым ящикам или не перемещаются в архивные почтовые ящики, проверьте следующее:

**Корневые причины:**

- **Помощник управляемой папки** не обрабатывал почтовый ящик пользователя. Помощник управляемых папок пытается обрабатывать каждый почтовый ящик в облачной организации один раз в семь дней.

  **Решение:** Запустите помощник управляемой папки.

- **Удержание** в **почтовом** ящике включено. Если почтовый ящик размещен на удержании, политика хранения в почтовом ящике не будет обработана в течение этого времени.

  **Решение:** Проверьте состояние параметра удержания хранения и обновления по мере необходимости. Подробные сведения см. [в материале Удержание хранения почтовых ящиков.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Примечание:** Если размер почтового ящика меньше 10 МБ, помощник управляемых папок не будет автоматически обрабатывать почтовый ящик.
 
Дополнительные сведения о политиках хранения в центре администрирования Exchange см. в этой информации:

- [Теги хранения и политики хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Применить политику хранения к почтовым ящикам или](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [добавить или удалить теги хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Как определить тип удержания, примененного для почтового ящика](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

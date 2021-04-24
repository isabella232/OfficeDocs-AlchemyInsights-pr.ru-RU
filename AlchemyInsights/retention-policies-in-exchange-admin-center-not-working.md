---
title: Политики хранения в Центре администрирования Exchange не работают
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952241"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Политики хранения в Центре администрирования Exchange

Если вы хотите, чтобы мы запускали автоматические проверки указанных ниже параметров, выберите кнопку < -- в верхней части этой страницы, а затем введите адрес электронной почты пользователя, у которого возникли проблемы с политиками хранения.

Если у вас возникли проблемы с политиками хранения в Центре администрирования Exchange, которые не применяются к почтовым ящикам или не перемещаются в архивный почтовый ящик, проверьте следующее:

**Корневые причины:**

- **Помощник управляемой папки** не обрабатывал почтовый ящик пользователя. Помощник управляемых папок пытается обрабатывать каждый почтовый ящик в облачной организации один раз в семь дней.

  **Решение:** Запустите помощник управляемой папки.

- **Удержание** в **почтовом** ящике включено. Если почтовый ящик размещен на удержании, политика хранения в почтовом ящике не будет обработана в течение этого времени.

  **Решение:** Проверьте состояние параметра удержания хранения и обновления по мере необходимости. Подробные сведения см. [в материале Удержание хранения почтовых ящиков.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Примечание:** Если размер почтового ящика меньше 10 МБ, помощник управляемых папок не будет автоматически обрабатывать почтовый ящик.
 
Дополнительные сведения о политиках хранения в Центре администрирования Exchange см. в рублях:

- [Теги хранения и политики хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Применить политику хранения к почтовым ящикам или](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [добавить или удалить теги хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Как определить тип удержания, примененного для почтового ящика](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

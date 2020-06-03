---
title: Политики хранения в центре администрирования Exchange не работают
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502620"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Политики хранения в центре администрирования Exchange

 **Вопрос:** Новые или обновленные политики хранения в центре администрирования Exchange не применяются к почтовым ящикам, а элементы не перемещаются в архивный почтовый ящик или не удаляются. 
  
 **Основные причины:**
  
- Это может быть вызвано тем, что помощник по работе с **управляемыми папками** не обработал почтовый ящик пользователя. Помощник по работе с управляемыми папками пытается обрабатывать все почтовые ящики в облачной организации каждые семь дней. Если вы измените тег хранения или примените другую политику хранения к почтовому ящику, вы можете дождаться обработки почтового ящика помощником для управляемых папок или запустить командлет Start-ManagedFolderAssistant, чтобы запустить помощник по работе с управляемыми папками для обработки определенного почтового ящика. Выполнение этого командлета полезно для тестирования или устранения неполадок с политикой хранения или параметрами тегов хранения. Для получения дополнительных сведений посетите страницу [Запуск помощника для управляемых папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Решение:** Выполните следующую команду, чтобы запустить помощник по работе с управляемыми папками для определенного почтового ящика:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Это также может произойти, если **ретентионхолд** был **включен** для почтового ящика. Если почтовый ящик был включен в Ретентионхолд, политика хранения в почтовом ящике не будет обработана в течение этого времени. Дополнительные информатон для параметра Ретентионхолд: [удержание для хранения почтовых ящиков](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Решению**
    
  - Проверьте состояние параметра Ретентионхолд в определенном почтовом ящике в [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Выполните следующую команду, чтобы **Отключить** ретентионхолд для определенного почтового ящика:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Теперь повторно запустите помощник по работе с управляемыми папками:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Примечание:** Если размер почтового ящика не превышает 10 МБ, помощник по работе с управляемыми папками не будет автоматически обрабатывать этот почтовый ящик.
 
Более подробную информацию о политиках хранения в центре администрирования Exchange можно узнать в следующих статьях:
- [Теги хранения и политики хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Применение политики хранения к почтовым ящикам](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Добавление и удаление тегов хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Как определить тип удержания, примененного для почтового ящика](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

---
title: Политики хранения в центре администрирования Exchange не работают
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761595"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Политики хранения в центре администрирования Exchange

 **Вопрос:** Новые или обновленные политики хранения в центре администрирования Exchange не применяются к почтовым ящикам, а элементы не перемещаются в архивный почтовый ящик или не удаляются. 
  
 **Основные причины:**
  
- Это может быть вызвано тем, что **помощник** по работе с управляемыми папками не обработал почтовый ящик пользователя. Помощник по работе с управляемыми папками пытается обрабатывать все почтовые ящики в облачной организации каждые семь дней. Если вы измените тег хранения или примените другую политику хранения к почтовому ящику, вы можете дождаться обработки почтового ящика помощником для управляемых папок или запустить командлет Start-ManagedFolderAssistant, чтобы запустить помощник по работе с управляемыми папками для обработки определенного электронной. Выполнение этого командлета полезно для тестирования или устранения неполадок с политикой хранения или параметрами тегов хранения. Для получения дополнительных сведений посетите страницу [Запуск помощника для управляемых папок](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Решение:** Выполните следующую команду, чтобы запустить помощник по работе с управляемыми папками для определенного почтового ящика: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Это также может произойти, если **ретентионхолд** был **включен** для почтового ящика. Если почтовый ящик был включен в Ретентионхолд, политика хранения в почтовом ящике не будет обработана в течение этого времени. Дополнительные информатон для параметра Ретентионхолд: [удержание для хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)почтовых ящиков.
    
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
  


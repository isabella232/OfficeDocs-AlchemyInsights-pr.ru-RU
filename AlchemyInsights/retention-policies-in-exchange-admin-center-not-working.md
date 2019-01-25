---
title: Политики хранения в центре администрирования Exchange не работает
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486719"
---
 **Проблема:** Вновь созданный или политики хранения обновленные в центре администрирования Exchange не применяются к почтовым ящикам или не перемещаются в архивный почтовый ящик или удалении элементов. 
  
 **Основные причины:**
  
- Возможно, **Помощника для управляемых папок** не обработал почтовый ящик пользователя. Помощник для управляемых папок пытается обработки всех почтовых ящиков в организации на основе облака один раз в неделю. Если тега хранения или изменения другую политику хранения к почтовому ящику, подождать Assist управляемых папок обрабатывается почтовый ящик или можно запустить командлет Start-ManagedFolderAssistant запуск помощника для управляемых папок для обработки определенного почтовый ящик. Выполнение этого командлета можно использовать для проверки или устранения неполадок политику хранения или параметры тегов хранения. Для получения дополнительных сведений посетите [Запуск помощника для управляемых папок](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Решения:** Выполните следующую команду для запуска помощника для управляемых папок для определенного почтового ящика: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Это может произойти при **RetentionHold** была **включена** для почтового ящика. Если поместил почтовый ящик на RetentionHold политики хранения для почтового ящика не будут обрабатываться в это время. Для более informaton о см параметр RetentionHold: [Удержание почтовых ящиков](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Решение**
    
  - Проверьте состояние параметра RetentionHold на определенного почтового ящика в [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Выполните следующую команду, чтобы **Отключить** RetentionHold на определенного почтового ящика. 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Повторно запустите управляемая папка помощник по:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Примечание:** Если почтовый ящик меньше 10 МБ, помощника для управляемых папок не будет обрабатывать автоматически почтового ящика. 
  


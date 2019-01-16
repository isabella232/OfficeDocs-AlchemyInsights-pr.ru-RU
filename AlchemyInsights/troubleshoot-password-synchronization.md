---
title: Устранение неполадок синхронизации паролей
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308725"
---
# <a name="troubleshoot-password-synchronization"></a>Устранение неполадок синхронизации паролей

Для устранения неполадок, которых нет пароли синхронизации с Azure AD подключить версии 1.1.614.0 или более поздней версии:
  
1. Откройте новый сеанс Windows PowerShell на сервере Azure AD подключиться с параметром **Запуск от имени администратора** . 
    
2. Запустите **командлет Set-ExecutionPolicy RemoteSigned** или **Set-ExecutionPolicy Unrestricted**. 
    
3. Запустите мастер подключения Azure AD.
    
4. Перейдите к ** дополнительные задачи ** выберите параметр ** Устранение ** и нажмите кнопку **Далее**. 
    
5. На странице "Устранение неполадок" щелкните меню **запуска, чтобы начать устранение неполадок** в PowerShell. 
    
6. В главном меню выберите **Устранение неполадок синхронизации паролей**. 
    
7. В меню sub выберите **синхронизации паролей вообще не работает**. 
    
 **Изучите результаты задачу по устранению неполадок**
  
Устранения неполадок задачи выполняются следующие проверки:
  
- Проверяет, что для вашего клиента Azure AD включена функция синхронизации паролей.
    
- Проверяет, что сервер подключить Azure AD не входит в режим временных файлов.
    
- Для каждого существующего локального Active Directory соединителя (который соответствует существующего леса Active Directory):
    
- 
  - Проверяет, что включен компонент синхронизации паролей.
    
  - Поиск события пульса синхронизации паролей в журнале событий приложений Windows.
    
  - Для каждого домена Active Directory в разделе локальный Соединитель Active Directory:
    
  - Проверяет доступность с Azure AD подключение сервера домена.
    
  - Проверяет, что учетные записи доменных служб Active Directory (AD DS), используется локальный Соединитель Active Directory имеет правильное имя пользователя, пароль и разрешения, необходимые для синхронизации паролей.
    
Дополнительные сведения об устранении проблем синхронизации паролей в разделе [Синхронизация паролей Устранение неполадок с синхронизацией подключить Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  


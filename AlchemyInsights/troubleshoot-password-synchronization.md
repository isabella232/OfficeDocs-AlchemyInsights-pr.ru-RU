---
title: Устранение неполадок при синхронизации паролей
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732523"
---
# <a name="troubleshoot-password-synchronization"></a>Устранение неполадок при синхронизации паролей

Устранение неполадок, в которых не синхронизируются пароли с Azure AD Connect версии 1.1.614.0 или более поздней.
  
1. Откройте новый сеанс Windows PowerShell на сервере Azure AD Connect с параметром **Запуск от имени администратора** .

2. Выполните командлет **Set — ExecutionPolicy RemoteSigned** или **Set/ExecutionPolicy Unrestricted**.

3. Запустите мастер Azure AD Connect.

4. Перейдите на страницу **Дополнительные задачи** , выберите **Устранение неполадок**и нажмите кнопку **Далее**.

5. На странице Устранение неполадок нажмите кнопку **запустить, чтобы запустить меню устранение неполадок** в PowerShell.

6. В главном меню выберите пункт **Устранение неполадок синхронизации паролей**.

7. Во вложенном меню выберите пункт **Синхронизация паролей не работает**.

**Общие сведения о результатах задачи "Устранение неполадок"**
  
Задача по устранению неполадок выполняет следующие проверки:
  
- Проверка включения функции синхронизации паролей для клиента Azure AD.

- Проверяет, находится ли сервер Azure AD Connect в режиме промежуточного хранения.

- Для каждого существующего локального соединителя Active Directory (соответствующего существующему лесу Active Directory):

- 
  - Проверяет, включена или отключена функция синхронизации паролей.

  - Выполняет поиск событий пульса синхронизации паролей в журналах событий приложений Windows.

  - Для каждого домена Active Directory в локальном соединителе Active Directory:

  - Проверяет, достижим ли домен с сервера Azure AD Connect.

  - Проверка того, что учетные записи доменных служб Active Directory (AD DS), используемые локальным соединителем Active Directory, имеют правильные имя пользователя, пароль и разрешения, необходимые для синхронизации паролей.

Дополнительные сведения об устранении неполадок при синхронизации паролей приведены [в разделе Устранение неполадок с синхронизацией паролей с помощью Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  
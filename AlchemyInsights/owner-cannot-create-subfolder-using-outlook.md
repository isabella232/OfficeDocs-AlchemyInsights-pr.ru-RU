---
title: Владелец не может создать вложенную папку с помощью Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665731"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Владелец не может создать вложенную папку с помощью Outlook

**Существует проблема с созданием вложенных папок владельцами общедоступных папок с помощью Outlook. Эта проблема будет скоро исправлена.**

Пока же используйте одно из следующих временных решений.

1. Для создания вложенных папок используйте Outlook для Mac, так как проблема затрагивает только Outlook для классических выпусков Windows (все версии)
2. Пусть вложенные папки создает администратор с помощью оболочки EXO или EAC
3. Измените параметр DefaultPublicFolderMailbox/EffectivePublicFolderMailbox пользователя на почтовый ящик, отличный от почтового ящика содержимого, в папке которого возникает проблема  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Подождите час и перезапустите клиент Outlook
---
title: Владелец не может создать вложенную папку с помощью Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063137"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Владелец не может создать вложенную папку с помощью Outlook

**Существует проблема с созданием вложенных папок владельцами общедоступных папок с помощью Outlook. Эта проблема будет скоро исправлена.**

Пока же используйте одно из следующих временных решений.

1. Для создания вложенных папок используйте Outlook для Mac, так как проблема затрагивает только Outlook для классических выпусков Windows (все версии)
2. Пусть вложенные папки создает администратор с помощью оболочки EXO или EAC
3. Измените параметр DefaultPublicFolderMailbox/EffectivePublicFolderMailbox пользователя на почтовый ящик, отличный от почтового ящика содержимого, в папке которого возникает проблема  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Подождите час и перезапустите клиент Outlook
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836148"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Владелец не может создать вложенную папку с помощью Outlook

**Существует проблема с созданием вложенных папок владельцами общедоступных папок с помощью Outlook. Эта проблема будет скоро исправлена.**

Пока же используйте одно из следующих временных решений.

1. Для создания вложенных папок используйте Outlook для Mac, так как проблема затрагивает только Outlook для классических выпусков Windows (все версии)
2. Пусть вложенные папки создает администратор с помощью оболочки EXO или EAC
3. Измените параметр DefaultPublicFolderMailbox/EffectivePublicFolderMailbox пользователя на почтовый ящик, отличный от почтового ящика содержимого, в папке которого возникает проблема  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Подождите час и перезапустите клиент Outlook
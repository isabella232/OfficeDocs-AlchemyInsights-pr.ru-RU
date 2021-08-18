---
title: Функция синхронизации контактов Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327346"
---
# <a name="teams-contacts-sync"></a>Функция синхронизации контактов Teams

Teams использует контакты в Active Directory организации и контакты, добавленные в папку Outlook пользователя по умолчанию. Если контакты не отображаются в Microsoft Teams, попробуйте выполнить следующие действия:

**Примечание.** Если информация об одном или нескольких контактах обновлялась недавно, синхронизация контактов может занять до 48 часов.

1. Выйдите из Teams и перезапустите. Проверьте, появляются ли ваши контакты.
1. Очистка кэша Teams:
    1. Перейдите в **%appdata%\Microsoft\Teams**.
    1. Удалите содержимое папки.
    1. Перезапустите компьютер и повторно запустите Teams.
1. Если контакт находится в Outlook, обязательно добавьте его в список контактов. В Outlook в адресной строке выберите **Файл**, а затем выберите **Добавить в контакты**.
1. Разместите почтовый ящик Exchange пользователя в сети (а не локально). Дополнительные сведения см. в статье [Взаимодействие Microsoft Teams и Exchange](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
1. Добавьте номер телефона контакта в контактные данные.
1. Выполните поиск электронной почты контакта на панели “Поиск”. Контакты, которые можно получить, синхронизированы со списком контактов.

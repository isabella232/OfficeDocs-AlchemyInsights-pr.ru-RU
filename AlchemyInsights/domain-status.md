---
title: Состояние домена . Не выбраны службы
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 2247da07d60431edef5b5dea8a5c06d51579008c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326590"
---
# <a name="domain-status---no-services-selected"></a>Состояние домена . Не выбраны службы

**Отсутствие выбранных** служб означает, что вы не выбрали какие-либо Microsoft 365, такие как Exchange Online, Skype для бизнеса или Intune, и управление мобильными устройствами для Microsoft 365 для использования с помощью настраиваемого домена. Если вы используете Exchange hybrid (Exchange с Exchange Online) или внешнюю фильтрацию нежелательной почты с Exchange и никакими другими службы Майкрософт, вы можете игнорировать это сообщение. Состояние здоровья домена доступно только для доменов, подключенных непосредственно к службе.

Чтобы выбрать службы для вашего домена:

1. Из **Параметры** доменов проверьте поле рядом с доменом с сообщением о состоянии  >  [](https://admin.microsoft.com/Adminportal/Home)Нет **выбранных служб.**
1. Выберите **Управление DNS для** запуска мастера настройки домена.
    - Если вы решите **добавить собственные записи DNS,** обязательно выберите службу по запросу. Дополнительные службы могут быть доступны в **расширенных параметрах**.
    - Если вы решите **добавить записи DNS** microsoft или дополнительные параметры Настройка моих онлайн-служб для меня, все доступные службы будут предложены и выбраны  >   автоматически.
1. Продолжайте через мастера, чтобы завершить установку DNS и выбор службы.
 
Дополнительные справки по настройке домена см. в [справке Добавить записи DNS для подключения домена.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)


---
title: Управление глобальным списком адресов и автономной адресной книгой организации
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812704"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Управление глобальным списком адресов (GAL) и автономной адресной книгой (OAB) организации

Глобальный список адресов (GAL) — это список объектов, поддерживающих почту (любой тип получателей, который может получать письма) в организации. В каждой организации автоматически создается один глобальный список адресов. Вы можете создавать дополнительные глобальные списки адресов, чтобы разделить пользователей по организациям или расположениям, но один пользователь может одновременно просматривать и использовать только один глобальный список адресов.

Некоторые почтовые клиенты, такие как Outlook для Windows, скачивают глобальный список адресов (GAL) для автономного использования. Это называется автономной адресной книгой (OAB). В Exchange Online автономная адресная книга обновляется каждые 8 часов, после чего клиенты должны скачать ее для обновления своей локальной копии OAB. Любые изменения получателей должны сначала отобразиться в GAL, чтобы затем внести их в OAB.

Некоторые распространенные процедуры GAL и OAB:

- По ряду причин вам может потребоваться скрыть некоторые объекты в глобальном списке адресов. Сведения см. в разделе [Скрытие получателей из списков адресов](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Если вам нужно предоставить определенным группам пользователей настроенные представления глобального списка адресов организации, см. статью [Политики адресных книг в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Создайте глобальный список адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), а чтобы узнать, как использовать разрешения GAL, см. статью [Списки адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Обратите внимание, что при создании GAL вам также может потребоваться создать OAB. См. статью [Процедуры автономной адресной книги](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).

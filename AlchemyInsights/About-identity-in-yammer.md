---
title: Сведения об удостоверениях в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664183"
---
# <a name="about-identity-in-yammer"></a>Сведения об удостоверениях в Yammer

Чтобы избежать проблем, связанных с удостоверениями, рекомендуется выполнить перечисленные ниже действия во всех сетях.

1. Используйте удостоверение Office 365 после подготовки учетных записей Microsoft 365 для пользователей в Azure AD, чтобы все пользователи могли входить в систему с помощью своей основной учетной записи Microsoft 365. Дополнительные сведения см. в статье [Использование удостоверения Office 365 для Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Объединение нескольких сетей Yammer. Устаревшие конфигурации Yammer позволяют подключаться к нескольким сетям Yammer с одним клиентом. Дополнительные сведения см. в статье [Сетевая миграция: объединение нескольких сетей Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Можно также применять лицензирование Yammer для блокировки пользователей из Yammer, если у них нет лицензии. Дополнительные сведения см. в статье [Управление лицензиями пользователей Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Наконец, проведите аудит списка пользователей для старых сетей Yammer и отключите прежних пользователей. Рекомендуется отключить (деактивировать) пользователей, не удаляя их, потому что удаление необратимо. Дополнительные сведения см. в статьях [Аудит пользователей Yammer в сетях, подключенных к Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) и [Удаление пользователей](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

С помощью этих действий можно также настроить сеть Yammer для основного режима в Microsoft 365. Дополнительные сведения см. в статье [Настройка сети Yammer для основного режима в Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).
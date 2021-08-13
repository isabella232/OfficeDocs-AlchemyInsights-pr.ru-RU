---
title: Проблема с группами безопасности
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925754"
---
# <a name="issue-with-security-groups"></a>Проблема с группами безопасности

**Если отображается сообщение об ошибке сети AADDS104**

Недопустимые правила группы безопасности сети являются наиболее частой причиной сетевых ошибок для доменных служб Azure Active Directory (AD DS). Группа безопасности для виртуальной сети должна разрешать доступ к определенным портам и протоколам. Если такие порты заблокированы, платформа Azure не сможет отслеживать или обновлять управляемые домены. Это также влияет на синхронизацию между службами Azure AD и Azure AD DS. Убедитесь, что порты по умолчанию открыты, чтобы избежать перерывов в обслуживании.

Сведения об устранении распространенных оповещений о проблемах, связанных с настройкой группы безопасности сети, см. в статье [Добавление и проверка групп безопасности](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).

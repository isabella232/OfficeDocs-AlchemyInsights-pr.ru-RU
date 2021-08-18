---
title: Настройка и увеличение жизненного цикла маркеров
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: ce100fcc2c62d62477f78e10b3cc9233fc2f5c5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329099"
---
# <a name="configure-and-extend-token-lifetimes"></a>Настройка и увеличение жизненного цикла маркеров

Вы можете указать жизненный цикл маркера доступа, SAML или идентификатора, выданного платформой удостоверений Майкрософт. Жизненный цикл маркера можно задать для всех приложений в вашей организации, мультитенантного приложения (охватывающего несколько организаций) или отдельного субъекта-службы в вашей организации. Дополнительные сведения см. в статье [Настраиваемые жизненные циклы маркера](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Например, см. статью [Примеры настройки жизненного цикла маркеров](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Сведения о настройке жизненного цикла и совместимости маркеров в Azure Active Directory B2C (Azure AD B2C), см. в статье [Настройка маркеров в Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Статья [Настройка сеанса в службе Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описывает методы единого входа (SSO), используемые в Azure AD B2C, и помогает выбрать подходящий способ единого входа при настройке политики.

**В течение какого времени действуют маркеры? В течение какого времени они действительны?**

Жизненный цикл маркеров составляет 1 час, а жизненный цикл сеанса — 24 часа. Это означает, что если запросы не были выполнены в течение 24 часов, перед запросом нового маркера потребуется выполнить вход еще раз.

**Примечание.** После 30 мая 2020 г. новый клиент не сможет использовать настраиваемую политику жизненных циклов маркеров для настройки сеанса и обновления маркеров. Прекращение поддержки происходит в течение нескольких месяцев. Это означает, что мы не будем учитывать существующие политики сеанса и обновления маркеров. Вы можете настроить жизненный цикл маркеров доступа после прекращение поддержки.







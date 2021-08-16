---
title: Подготовка пользователей из Workday в AD переходит в состояние карантина
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036505"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Подготовка пользователей из Workday в AD переходит в состояние карантина

**Подготовка пользователей из Workday в AD переходит в состояние карантина, и в AD не создаются пользователи**

Задание подготовки пользователей из Workday в AD перешло в состояние карантина, а в журналах аудита отображаются события сбоя экспорта с сообщением **Ошибка. OperationsError-SvcErr: произошла ошибка операции. Главная ссылка для службы каталогов не настроена. Таким образом, службе каталогов не удастся выдать ссылки на объекты вне этого леса**. Эта ошибка обычно возникает, если неправильно задано подразделение контейнера Active Directory или имеются проблемы с сопоставлением выражения, примененным для **parentDistinguishedName**.

Проверьте, нет ли опечаток в подразделении по умолчанию для параметра **Новые пользователи**. Убедитесь, что указанное подразделение уже существует в AD. Если вы используете атрибут **parentDistinguishedName** в сопоставлении атрибутов, убедитесь, что он всегда оценивается по известному контейнеру в домене AD. Проверьте событие экспорта в журналах аудита, чтобы увидеть созданное значение.

Дополнительные сведения о настройке Workday для автоматической подготовки см. в статье [Руководство по настройке Workday для автоматической подготовки пользователей](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).


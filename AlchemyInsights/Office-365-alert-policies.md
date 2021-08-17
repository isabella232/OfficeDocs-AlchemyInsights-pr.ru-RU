---
title: Политики 1385-Office-365-alert-
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: f5109445530ec4cc4988fb9c5d37145c45794ced6920607ce6df85c6497c25ec
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891692"
---
# <a name="alert-policies"></a>Политики оповещений

Microsoft 365 содержит политики [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) оповещений по умолчанию, которые запускают оповещения для организаций с подпиской Microsoft 365 корпоративный или Microsoft 365 правительства США E1/G1, E3/G3 или E5/G5. Поэтому администраторы могут получать оповещение электронной почты, отправленное Office365Alerts@microsoft.com с строкой субъекта, например "Предупреждение о низкой степени тяжести: имя политики оповещения". Уведомления оповещений отправляются при запуске оповещений для общих действий, например при работе с пользователями:

- Создайте правила почтового ящика, которые перенадвигают электронную почту.
- Назначение разрешений их почтового ящика.
- Общий доступ или удаление большого количества файлов в SharePoint файле.
- Создание поиска об обнаружении и экспорт результатов поиска.

Чтобы просмотреть и действовать в оповещении:

1. Выполните одно из следующих действий:
   - В <https://compliance.microsoft.com> Центр соответствия требованиям Microsoft 365, перейдите к **оповещений**. Или, чтобы перейти непосредственно на страницу **Оповещений,** используйте <https://compliance.microsoft.com/compliancealerts> .
   - На портале <https://security.microsoft.com> Microsoft 365 Defender, перейдите в **incidents & оповещений.** \>  Или, чтобы перейти непосредственно на страницу **Оповещений,** используйте <https://security.microsoft.com/alerts> .
2. Щелкните оповещение, чтобы отобразить страницу вылетов с информацией о оповещении.

Вы можете принять меры по оповещению, например удалить подозрительное правило [почтовых ящиков.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) Или вы можете просто закрыть оповещение, щелкнув **Разрешить** на странице вылет оповещения.

Дополнительные сведения о настройке и управлении политиками оповещения см. [в этой статье.](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)

**Важно:** уведомления электронной почты из Корпорации Майкрософт никогда не будут просить вас сделать следующее:

- Предоставление пароля
- Проверка сведений о безопасности учетной записи
- Повторное проверка подлинности

Если вы получаете сообщение электронной почты с такими запросами, оно не было отправлено Корпорацией Майкрософт и должно считаться фишинговой атакой. Если вы получаете сообщение с такими запросами, [ок. Сообщение в Корпорацию Майкрософт.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

---
title: Проблемы условного доступа
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069977"
---
# <a name="conditional-access-issues"></a>Проблемы условного доступа

**Устранение проблем с диагностикой входа**

Вы можете быстро узнать, что произошло или диагностировать проблемы, связанные с входом пользователя с помощью диагностики [входных данных:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Запустите Диагностику входа.
1. Найдите событие для анализа, введите сведения о пользователе, приложении, времени входа, id запроса или корреляции.
1. Просмотрите результаты диагностики, показывающие сведения о том, что произошло и какие действия можно принять для внесения изменений (если необходимы какие-либо изменения).

**Действия по устранению неполадок при входе** 

1. Перейдите на страницу Вход в Azure AD.
1. Фильтрация входов пользователя, диапазона времени, приложения, состояния, клиентского приложения и так далее.
1. Выберите событие входной точки и просмотреть вкладку Условный доступ, чтобы узнать, какие политики были оценены.
1. Щелкните строку политики, чтобы просмотреть сведения о политике и понять, почему она применяется.

**Средства устранения неполадок политики условного доступа**

- Режим только для отчетов позволяет оценить политику, не влияя на пользователей.
- Средство What-if позволяет смоделировать события регистрации и посмотреть, какие политики применяются.
- Аналитика и отчетная книга отображает влияние каждой политики в режиме реального времени.

**Политики базовой защиты**

Политики базовой защиты были обесценимы. Они больше не применяются и скоро будут удалены с портала Azure. Рекомендуется включить [по умолчанию безопасность.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Дополнительные сведения о условном доступе см. в этой информации:

[Наилучшие методы для условного доступа в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Элементы управления в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Расположения в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)

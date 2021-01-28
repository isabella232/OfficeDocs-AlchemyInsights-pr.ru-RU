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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013978"
---
# <a name="conditional-access-issues"></a>Проблемы условного доступа

**Устранение проблем с диагностикой входа**

Вы можете быстро узнать, что произошло или диагностировать проблемы, связанные с входом пользователя, с помощью диагностики [при входе:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Запустите Диагностику входа.
1. Найдите событие для анализа, введите сведения о пользователе, приложении, времени входа, ид запроса или ид корреляции.
1. Просмотрите результаты диагностики с подробными сведениями о том, что произошло и какие действия можно принять для внесения изменений (если необходимы какие-либо изменения).

**Действия по устранению неполадок при входе** 

1. Перейдите на страницу входов в Azure AD.
1. Фильтрация входов по пользователю, диапазону времени, приложению, статусу, клиентского приложения и так далее.
1. Выберите событие для регистрации и переберись на вкладку "Условный доступ", чтобы узнать, какие политики были оценены.
1. Щелкните строку политики, чтобы просмотреть сведения о политике и понять, почему она применяется.

**Средства устранения неполадок политики условного доступа**

- Режим только для отчетов позволяет оценить политику, не влияя на пользователей.
- Средство "что-если" позволяет имитировать события входов и видеть, какие политики применяются.
- В книге "Анализ и отчеты" отображается влияние каждой политики в режиме реального времени.

**Базовые политики защиты**

Политики базовой защиты были неподготовлены. Они больше не применяются и скоро будут удалены с портала Azure. Мы рекомендуем включить [значения по умолчанию для системы безопасности.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Дополнительные сведения об условном доступе см. в:

[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия условного доступа](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Элементы управления в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Расположения в условном доступе](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)

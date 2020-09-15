---
title: Миграция с AIP на MIP/унифицированные метки в Центре соответствия требованиям
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674339"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Миграция с AIP на MIP/унифицированные метки в Центре соответствия требованиям

Чтобы перейти с меток AIP на унифицированные метки в Центре безопасности и соответствия требованиям, выполните следующие действия.

**Активация защиты из портала Azure**

1. Если вы этого еще не сделали, откройте новое окно браузера и [войдите на портал Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Перейдите к колонке **Azure Information Protection**. Например, в главном меню щелкните **Все службы** и начните вводить **Information** в поле фильтра. Выберите **Azure Information Protection**. Если вы ранее не обращались к колонке Azure Information Protection, ознакомьтесь с однократными [дополнительными действиями](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) по ее добавлению на портал. Чтобы открыть колонку Azure Information Protection, у вас должен быть [план Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)или план Office 365, включающий управление правами. Если у вас есть одна из этих подписок, но появляется сообщение об отсутствии надлежащей подписки, [обратитесь в службу поддержки Майкрософт](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или используйте стандартные каналы поддержки.

2. Найдите параметры меню **Управление** и выберите **Активация защиты**. Щелкните **Активировать** и подтвердите действие. После завершения активации на информационной панели отобразится сообщение **Активация успешно завершена**.

**Перенос меток Azure Information Protection в Центр безопасности и соответствия требованиям Office 365**

1. Войдите в качестве пользователя с разрешениями глобального администратора.

2. Перейдите к колонке **Azure Information Protection**.

3. В меню **Управление** выберите параметр **Унифицированные метки**.

4. В колонке **Azure Information Protection — Унифицированные метки** щелкните **Активировать** и следуйте инструкциям в Интернете.

**Примечание**. Проверьте наличие соответствующих разрешений перед активацией миграции в Центр безопасности и соответствия требованиям. Дополнительные сведения см. в следующих статьях:

1. [Необходимо ли быть глобальным администратором для настройки Azure Information Protection? Или выполнение этой задачи можно делегировать другим администраторам?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важные сведения об административных ролях после миграции в Центр безопасности и соответствия требованиям](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles).

Дополнительные сведения о миграции с AIP на унифицированные метки в Центре безопасности и соответствия требованиям см. в статье [Перенос меток](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).

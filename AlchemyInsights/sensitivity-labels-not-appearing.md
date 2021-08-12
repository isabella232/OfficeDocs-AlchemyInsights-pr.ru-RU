---
title: Метки чувствительности, которые не отображаются
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061445"
---
# <a name="sensitivity-labels-not-appearing"></a>Метки чувствительности, которые не отображаются

Метки конфиденциальности позволяют классифицировать и защищать конфиденциальный контент. Они могут быть созданы в центре Центр соответствия требованиям Microsoft 365, Microsoft 365 безопасности или в центре Microsoft 365 безопасности & в соответствии с метами Classification > Sensitivity. Дополнительные сведения об этой функции см. в [обзоре меток конфиденциальности.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Если вы настроили метки конфиденциальности, но они не отображаются в Microsoft 365 приложениях, проверьте следующее:

- Подтверди, что метка конфиденциальности [была опубликована](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) пользователям и группам, которые вам нужны.

- Подтверждение того, что пользователь использует приложение, которое поддерживает метки чувствительности, см. в документе [метки конфиденциальности.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Если вы переносят [метки Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)будьте в курсе перечисленных [здесь соображений.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Поддержка защиты от потери данных(DLP): В настоящее время в политиках DLP можно использовать только метки хранения.  Поддержка меток конфиденциальности в политике DLP еще недоступна, но мы работаем над ней.

- Если шифрование включено на мете конфиденциальности, вы можете выбрать:
    - Назначение разрешений
    - Предоставление пользователям возможности назначать разрешения


Дополнительные сведения о возможных проблемах см. в выпуске [Known issues with sensitivity labels.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)
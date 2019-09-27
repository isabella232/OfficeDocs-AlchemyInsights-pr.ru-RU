---
title: Метки конфиденциальности не отображаются
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207238"
---
# <a name="sensitivity-labels-not-appearing"></a>Метки конфиденциальности не отображаются

Метки конфиденциальности позволяют классифицировать и защищать конфиденциальное содержимое. Они могут быть созданы в центре соответствия требованиям Microsoft 365, центре безопасности 365 Майкрософт или Office 365 центр соответствия требованиям & безопасности в разделе классификация > меток конфиденциальности. Чтобы узнать больше об этой функции, просмотрите раздел [Обзор меток конфиденциальности](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Если вы настроили метки конфиденциальности, но они не отображаются в приложениях Office, проверьте следующее:

- Убедитесь, что метка конфиденциальности была [опубликована](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) для нужных пользователей и групп.

- Убедитесь, что пользователь использует приложение, которое поддерживает метки чувствительности — просмотрите [метки конфиденциальности в документе](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Если вы переносите [метки Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), учитывайте вопросы, приведенные в [этой статье](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Поддержка защиты от потери данных (DLP): в настоящее время в качестве условия в политиках защиты от потери данных можно использовать только метки хранения.  Поддержка меток конфиденциальности в политике DLP пока недоступна, но мы работаем над этим.

- Если для метки конфиденциальности включено шифрование, вы можете выбрать один из следующих вариантов:
    - Назначить разрешения сейчас
    - Разрешить пользователям назначать разрешения


Дополнительные сведения о возможных проблемах приведены в статье [Известные проблемы с метками чувствительности](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).
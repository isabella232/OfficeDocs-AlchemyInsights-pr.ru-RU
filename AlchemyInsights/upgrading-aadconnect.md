---
title: 932 Обновление AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104825"
---
# <a name="upgrade-azure-ad-connect"></a>Обновление azure AD Подключение

По умолчанию автоматическое обновление включено для azure AD Подключение, что позволяет обеспечить запуск последней версии. Чтобы проверить параметры автоматического обновления, используйте **cmdlet Get-ADSyncAutoUpgrade** в Azure AD PowerShell. В cmdlet возвращается одно из следующих значений:

- **Включено.** Включено автоматическое обновление.

- **Отключено.** Автоматическое обновление отключено.

- **Приостановлено.** Система больше не имеет права получать автоматические обновления. Вы не можете настроить это значение; она установлена системой.

Дополнительные сведения см. в [автоматическом обновлении.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Чтобы скачать последнюю версию Azure AD Подключение, перейдите к [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .

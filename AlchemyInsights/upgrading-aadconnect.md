---
title: 932 обновление AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365922"
---
# <a name="upgrade-azure-ad-connect"></a>Обновление Azure AD Connect

По умолчанию автоматическое обновление включено для Azure AD Connect, что позволяет убедиться, что вы используете последнюю версию. Чтобы проверить параметры автоматического обновления, используйте командлет **Get – адсинкаутаупграде** в Azure AD PowerShell. Командлет возвращает одно из следующих значений:

- **Enabled**: автоматическое обновление включено.

- **Disabled**: автоматическое обновление отключено.

- **Suspended**: система больше не имеет права на получение автоматических обновлений. Вы не можете настроить это значение; Он задается системой.

Более подробную информацию можно узнать в статье [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Чтобы скачать последнюю версию Azure AD Connect, перейдите по [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)адресу.

---
title: 932 обновление AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806052"
---
# <a name="upgrade-azure-ad-connect"></a>Обновление Azure AD Connect

По умолчанию автоматическое обновление включено для Azure AD Connect, что позволяет убедиться, что вы используете последнюю версию. Чтобы проверить параметры автоматического обновления, используйте командлет **Get – адсинкаутаупграде** в Azure AD PowerShell. Командлет возвращает одно из следующих значений:

- **Enabled**: автоматическое обновление включено.

- **Disabled**: автоматическое обновление отключено.

- **Suspended**: система больше не имеет права на получение автоматических обновлений. Вы не можете настроить это значение; Он задается системой.

Более подробную информацию можно узнать в статье [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Чтобы скачать последнюю версию Azure AD Connect, перейдите по адресу [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .

---
title: 932 обновление AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389750"
---
# <a name="upgrade-azure-ad-connect"></a>Обновление Azure AD Connect

По умолчанию автоматическое обновление включено для Azure AD Connect, что позволяет убедиться, что вы используете последнюю версию. Чтобы проверить параметры автоматического обновления, используйте командлет **Get – адсинкаутаупграде** в Azure AD PowerShell. Командлет возвращает одно из следующих значений: 

- **Enabled**: автоматическое обновление включено.

- **Disabled**: автоматическое обновление отключено.

- **Suspended**: система больше не имеет права на получение автоматических обновлений. Вы не можете настроить это значение; Он задается системой. 

Более подробную информацию можно узнать в статье [Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Чтобы скачать последнюю версию Azure AD Connect, перейдите по [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)адресу.

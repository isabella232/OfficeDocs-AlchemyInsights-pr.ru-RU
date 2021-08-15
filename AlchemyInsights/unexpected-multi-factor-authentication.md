---
title: Внеплановая многофакторная проверка подлинности
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: d2b97175049bd9732b7444b029f7ea8610c3d5a2c02878ec5f20ded916baadd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53991152"
---
# <a name="unexpected-multi-factor-authentication"></a>Внеплановая многофакторная проверка подлинности

Если ваш клиент был создан позднее 21 октября 2019 г. и вам неожиданно предлагают пройти MFA, скорее всего, в вашем клиенте включены [параметры безопасности по умолчанию](https://aka.ms/securitydefaults). 

Для управления параметрами безопасности по умолчанию:

1. Войдите в [Центр администрирования](https://go.microsoft.com/fwlink/p/?linkid=834822) с учетными данными глобального администратора.

2. Перейдите в раздел [Свойства Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. В нижней части страницы щелкните **Управление параметрами безопасности по умолчанию**.

4. Нажмите кнопку **Да**, чтобы включить параметры безопасности по умолчанию, или **Нет**, чтобы их отключить.

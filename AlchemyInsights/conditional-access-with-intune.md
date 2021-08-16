---
title: Условный доступ с intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069725"
---
# <a name="conditional-access-with-intune"></a>Условный доступ с intune

Использование  **условного доступа**  с помощью Intune требует 3 действия:

- Создайте **политику** соответствия требованиям [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS, Windows)](https://docs.microsoft.com/intune/compliance-policy-create-ios) [для](https://docs.microsoft.com//intune/compliance-policy-create-windows)определения параметров, которые необходимо соблюдать, прежде чем устройство будет считаться совместимым. Например, устройство должно иметь пин-код не менее 6 цифр, прежде чем считать его совместимым.
- Создайте **политику условного**  доступа, которая определяет, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.  [Например, устройство](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  должно быть совместимым перед доступом к корпоративной электронной почте.
- Убедитесь, что  политики соответствия **требованиям** и политики условного доступа ориентированы на желаемые группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.

**Полезные ссылки:**

[Обзор соответствия требованиям устройств](https://docs.microsoft.com/intune/device-compliance-get-started)

[Устранение неполадок в ЦС](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Политика устранения неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Чтобы защитить электронную почту (Exchange в Интернете) от доступа с помощью некомплиентных устройств, необходимо следовать обоим документам:

1. [Защита доступа к электронной почте с устройств с помощью EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Защита доступа к электронной почте с устройств с помощью современных клиентов проверки подлинности, таких как Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)
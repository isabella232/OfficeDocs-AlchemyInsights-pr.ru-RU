---
title: Условный доступ с помощью Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931449"
---
# <a name="conditional-access-with-intune"></a>Условный доступ с помощью Intune

Для использования **условного доступа** в Intune необходимо 3 этапа:

- Создайте **политику соответствия требованиям** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), чтобы определить параметры, которые должны быть выполнены до того, как устройство считается совместимым. Например, устройство должно иметь ПИН-код как минимум до 6 цифр, прежде чем он будет признан совместимым.
- Создайте **политику условного доступа** , определяющую, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам.  [Например,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) устройство должно быть совместимо перед доступом к корпоративной почте.
- Убедитесь, что **политики соответствия требованиям** и политики **условного доступа** нацелены на нужные группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.

**Полезные ссылки:**

[Обзор соответствия требованиям устройств](https://docs.microsoft.com/intune/device-compliance-get-started)

[Устранение неполадок ЦС](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Политика устранения неполадок](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Чтобы защитить электронную почту (Exchange Online) от доступа несоответствующих требованиям устройств, необходимо следовать обоим документам:

1. [Защита доступа к электронной почте с устройств, использующих EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Защита доступа к электронной почте с устройств с помощью современных клиентов проверки подлинности, таких как Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)
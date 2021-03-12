---
title: Использование условного доступа с помощью Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737582"
---
# <a name="using-conditional-access-with-intune"></a>Использование условного доступа с помощью Intune

Использование условного доступа с помощью Intune требует 3 действия:

- [Создайте политику соответствия требованиям, чтобы определить параметры, которые должны быть выполнены до того, как устройство будет считаться совместимым. Например, устройство должно иметь пин-код не менее 6 цифр, прежде чем считать его совместимым.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Создайте политику условного доступа, которая определяет, какие ресурсы защищены и какие условия должны быть выполнены для доступа к этим ресурсам. Например, устройство должно быть совместимым перед доступом к корпоративной электронной почте.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Убедитесь, что политики соответствия требованиям и политики условного доступа ориентированы на желаемые группы пользователей. Для этого может потребоваться создание определенных групп пользователей в Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Дополнительные сведения](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)

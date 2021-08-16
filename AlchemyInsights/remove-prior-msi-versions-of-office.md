---
title: Удаление предыдущих версий MSI Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 45e3cac521bc1c2a90dc7d3ddd4958233c3cf7bbd2ea007e581f343bca7b5631
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023787"
---
# <a name="remove-prior-msi-versions-of-office"></a>Удаление предыдущих версий MSI Office

Перед установкой Windows (MSI) рекомендуется удалить Office версии Office 365 профессиональный плюс. Вот как это сделать:

1. Если для установки Office MSI используется средство развертывания Office (ODT), чтобы удалить Office. Элемент RemoveMSI можно использовать в **configuration.xml** файле.
1. Следуйте инструкциям в этой статье: [Office 365 безопасности & Центра соответствия требованиям.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
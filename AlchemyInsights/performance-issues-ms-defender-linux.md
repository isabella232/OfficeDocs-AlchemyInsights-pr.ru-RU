---
title: Проблемы с производительностью Microsoft Defender для конечной точки в Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 26ad9631111c250fd8b9ec32d4a6122f37f82513b7542231e402317aea4949dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899413"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Проблемы с производительностью Microsoft Defender для конечной точки в Linux

В этой статье описаны действия по выявлению проблем с производительностью Microsoft Defender для конечной точки в Linux.

Сначала необходимо убедиться, что проблема, с которой вы столкнулись, устранена в [последней версии](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Прежде чем приступить к исследованию, см. статью [Устранение неполадок с производительностью Microsoft Defender для конечной точки в Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Исключения

Исключения могут помочь устранить проблемы с производительностью. Прежде чем приступить к работе, просмотрите исключения, чтобы выявить и задокументировать любой дополнительный риск.

Дополнительные сведения см. в статье [Настройка и проверка исключений Microsoft Defender для конечной точки в Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-exclusions).

Если необходимо исключить несколько файлов и папок, которые находятся в одной точке подключения, рекомендуется исключить точку подключения. Начиная с февральского выпуска 101.22.80, вы сможете исключить всю точку подключения.

Например, если /mnt/backup является точкой подключения, вы можете добавить /mnt/backup в список исключений, выполнив следующую команду:

`$ mdatp exclusion folder add –path /mnt/backup`

**Примечание**. Добавление исключений увеличивает риск неполного обнаружения вредоносных программ, поэтому их следует применять с осторожностью.

## <a name="need-help"></a>Нужна помощь?

Чтобы мы могли вам оказать более эффективную помощь, соберите диагностические данные перед обращением в службу поддержки.

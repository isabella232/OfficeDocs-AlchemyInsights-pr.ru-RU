---
title: Проблема очереди печати устранена
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911351"
---
# <a name="print-spooler-issue-is-resolved"></a>Проблема очереди печати устранена

Если ваше устройство обновлено до Windows 10 **сборка ОС 19041.329**, у вас могла возникать проблема, из-за которой не удавалось выполнить печать на некоторых принтерах. При попытке печати очередь печати принтера может отображать ошибку или неожиданно закрываться, при этом на затронутом принтере не выполняется печать. Эта проблема устранена в сборке ОС **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Текущее исследование**

Файл службы LSASS (**Isass.exe**) может приводить к сбою на некоторых устройствах с сообщением об ошибке "В важном системном процессе C:\WINDOWS\system32\lsass.exe возник сбой с кодом состояния c0000008. Требуется перезагрузить компьютер".  **Корпорация Майкрософт работает над решением и предоставит обновление в ближайшем выпуске.**

Дополнительные сведения см. в статье [Известные проблемы с Windows 10 версии 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).
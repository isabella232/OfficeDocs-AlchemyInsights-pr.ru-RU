---
title: Проблема очереди печати устранена
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083981"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="2699b-102">Проблема очереди печати устранена</span><span class="sxs-lookup"><span data-stu-id="2699b-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="2699b-103">Если ваше устройство обновлено до Windows 10 **сборка ОС 19041.329**, у вас могла возникать проблема, из-за которой не удавалось выполнить печать на некоторых принтерах.</span><span class="sxs-lookup"><span data-stu-id="2699b-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="2699b-104">При попытке печати очередь печати принтера может отображать ошибку или неожиданно закрываться, при этом на затронутом принтере не выполняется печать.</span><span class="sxs-lookup"><span data-stu-id="2699b-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="2699b-105">Эта проблема устранена в сборке ОС **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="2699b-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="2699b-106">**Текущее исследование**</span><span class="sxs-lookup"><span data-stu-id="2699b-106">**Ongoing investigation**</span></span>

<span data-ttu-id="2699b-107">Файл службы LSASS (**Isass.exe**) может приводить к сбою на некоторых устройствах с сообщением об ошибке "В важном системном процессе C:\WINDOWS\system32\lsass.exe возник сбой с кодом состояния c0000008.</span><span class="sxs-lookup"><span data-stu-id="2699b-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="2699b-108">Требуется перезагрузить компьютер".</span><span class="sxs-lookup"><span data-stu-id="2699b-108">The machine must now be restarted".</span></span>  <span data-ttu-id="2699b-109">**Корпорация Майкрософт работает над решением и предоставит обновление в ближайшем выпуске.**</span><span class="sxs-lookup"><span data-stu-id="2699b-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="2699b-110">Дополнительные сведения см. в статье [Известные проблемы с Windows 10 версии 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="2699b-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>
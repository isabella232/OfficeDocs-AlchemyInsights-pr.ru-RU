---
title: Устранение неполадок при зависании задания службы импорта
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059852"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="ff004-102">Устранение неполадок при зависании задания службы импорта</span><span class="sxs-lookup"><span data-stu-id="ff004-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="ff004-103">Если у вас возникли проблемы с зависанием или сбоем заданий службы импорта, изучите и попробуйте выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="ff004-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="ff004-104">Проверьте размер PST-файла.</span><span class="sxs-lookup"><span data-stu-id="ff004-104">Review the size of of the PST file.</span></span> <span data-ttu-id="ff004-105">Максимальный рекомендуемый размер PST-файла для импорта составляет 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ff004-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="ff004-106">Если вы подозреваете, что элементы пропущены из-за повреждения, запустите Scanpst.exe, чтобы диагностировать и исправить ошибки в PST-файлах.</span><span class="sxs-lookup"><span data-stu-id="ff004-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="ff004-107">Если во время импорта вы видите ошибку MapiExceptionShutoffQuotaExceeded, убедитесь, что емкость целевого почтового ящика достаточна для импорта нужных PST-файлов.</span><span class="sxs-lookup"><span data-stu-id="ff004-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="ff004-108">Дополнительные сведения об устранении проблем с заданиями импорта PST-файлов см. в статье [Устранение проблем с заданиями импорта PST-файлов](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="ff004-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="ff004-109">Сведения о том, как устранять проблемы при импорте PST-файлов в Outlook, см. в статье [Устранение проблем с импортом PST-файла Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="ff004-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>
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
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105113"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Устранение неполадок при зависании задания службы импорта

Если у вас возникли проблемы с зависанием или сбоем заданий службы импорта, изучите и попробуйте выполнить следующие действия.

- Проверьте размер PST-файла. Максимальный рекомендуемый размер PST-файла для импорта составляет 20 ГБ.

- Если вы подозреваете, что элементы пропущены из-за повреждения, запустите Scanpst.exe, чтобы диагностировать и исправить ошибки в PST-файлах.

- Если во время импорта вы видите ошибку MapiExceptionShutoffQuotaExceeded, убедитесь, что емкость целевого почтового ящика достаточна для импорта нужных PST-файлов.

Дополнительные сведения об устранении проблем с заданиями импорта PST-файлов см. в статье [Устранение проблем с заданиями импорта PST-файлов](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Сведения о том, как устранять проблемы при импорте PST-файлов в Outlook, см. в статье [Устранение проблем с импортом PST-файла Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).
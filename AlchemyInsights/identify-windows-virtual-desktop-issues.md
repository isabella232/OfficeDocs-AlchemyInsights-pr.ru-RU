---
title: Выявление проблем Виртуального рабочего стола Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590298"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Выявление проблем Виртуального рабочего стола Windows

Служба диагностики Виртуального рабочего стола Windows использует только один командлет PowerShell, но содержит множество дополнительных параметров, позволяющих сузить круг проблем и изолировать их. Чтобы начать, выполните указанные ниже действия. 

1. Скачайте и импортируйте модуль PowerShell для Виртуального рабочего стола Windows. Дополнительные сведения см. в статье [Командлеты Виртуального рабочего стола Windows для Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Запустите следующий командлет, чтобы войти в свою учетную запись:
    
    Пример: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**ПРИМЕЧАНИЕ.** Все запросы, использующие PowerShell, должны включать параметры -UserName или -ActivityID. Дополнительные сведения о возможностях мониторинга см. в статье [Использование службы аналитики журналов в целях диагностики](https://go.microsoft.com/fwlink/?linkid=2126847).

Чтобы отфильтровать диагностические действия по пользователям, выполните следующий командлет:

Пример: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Для диагностики проблем можно использовать имеющийся список фильтров. Дополнительные сведения о диагностике проблем см. в статье [Выявление и диагностика проблем Виртуального рабочего стола Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Дополнительные сведения о распространенных ошибках см. в разделе [Распространенные сценарии ошибок](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).

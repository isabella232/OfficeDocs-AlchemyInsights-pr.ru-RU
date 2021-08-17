---
title: Средство диагностики служб для Виртуального рабочего стола Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: e6c20af2c3fc54b203f3bda5c0c0f00faacd92800566bd507867c4e9fe4a23f1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052327"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Средство диагностики служб для Виртуального рабочего стола Windows

Виртуальный рабочий стол Windows (WVD) предоставляет средство диагностики, позволяющее администраторам выявлять ошибки в едином интерфейсе. Это средство регистрирует диагностические данные, каждый раз, когда WVD используется пользователем, которому назначена роль WVD. Каждый журнал содержит сведения о роли WVD, связанной с определенными действиями, сообщения об ошибках, отображающиеся во время сеанса, а также сведения о клиенте и пользователе. Чтобы настроить службу аналитики журналов Azure для записи журнала действий, созданного средством диагностики, выполните следующие действия.

1. Создайте рабочую область службы аналитики журналов с помощью [портала Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [Подключите компьютеры с Windows к Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Получите идентификатор и первичный ключ рабочей области. Эти данные необходимы мастеру установки, чтобы правильно настроить агент и обеспечить его связь с Azure Monitor.

1. [Перенесите диагностические данные в рабочую область](https://go.microsoft.com/fwlink/?linkid=2128284). Вы можете перенести диагностические данные из клиента WVD в службу аналитики журналов для вашей рабочей области.

1. [Выполните поиск и диагностику](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблем, которые являются внутренними или внешними по отношению к WVD.

Дополнительные сведения о настройке средства диагностики служб для WVD см. в статье "Использование службы аналитики журналов в целях диагностики".
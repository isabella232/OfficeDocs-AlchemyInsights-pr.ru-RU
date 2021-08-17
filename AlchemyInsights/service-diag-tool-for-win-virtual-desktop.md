---
title: Средство диагностики служб для Виртуального рабочего стола Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052399"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Средство диагностики служб для Виртуального рабочего стола Windows

Виртуальный рабочий стол Windows (WVD) предоставляет средство диагностики, позволяющее администраторам выявлять ошибки в едином интерфейсе. Это средство регистрирует диагностические данные, каждый раз, когда WVD используется пользователем, которому назначена роль WVD. Каждый журнал содержит сведения о роли WVD, связанной с определенными действиями, сообщения об ошибках, отображающиеся во время сеанса, а также сведения о клиенте и пользователе. Azure Log Analytics можно настроить для захвата журнала действий, созданного диагностическим средством. Вот как это сделать:

1. Создайте рабочую область службы аналитики журналов с помощью [портала Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Подключите компьютеры с Windows к Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Получите идентификатор и первичный ключ рабочей области. Эти данные необходимы мастеру установки, чтобы правильно настроить агент и обеспечить его связь с Azure Monitor.
1. [Перенесите диагностические данные в рабочую область](https://go.microsoft.com/fwlink/?linkid=2128284). Вы можете перенести диагностические данные из клиента WVD в службу аналитики журналов для вашей рабочей области.
1. [Определение и диагностика](https://go.microsoft.com/fwlink/?linkid=2128338) внутренних или внешних проблем по отношению к WVD.

Дополнительные данные о настройке средства диагностики служб для WVD см. в [журнале Use Log Analytics для](https://go.microsoft.com/fwlink/?linkid=2128084)функции диагностики.

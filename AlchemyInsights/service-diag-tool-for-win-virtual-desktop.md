---
title: Средство диагностики служб для виртуального рабочего стола Windows
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665827"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Средство диагностики служб для виртуального рабочего стола Windows

Виртуальный рабочий стол Windows (WVD) предлагает средство диагностики, которое позволяет администраторам выявлять ошибки с помощью одного интерфейса. Это средство записывает в журнал сведения, связанные с диагностикой, каждый раз, когда WVD используется кем-то, кому назначена роль WVD. Каждый журнал содержит сведения о роли WVD, которая участвует в действии, сообщения об ошибках, которые отображаются во время сеанса, а также сведения о клиенте и пользователе. Azure Log Analytics можно настроить для записи журнала действий, созданного средством диагностики. Вот как это сделать:

1. Создайте рабочее пространство Log Analytics с помощью портала [Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Подключите компьютеры с Windows к Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Получите ИД рабочей области и первичный ключ рабочей области. Эти сведения необходимы мастеру настройки, чтобы правильно настроить агент и убедиться, что он может взаимодействовать с Azure Monitor.
1. [Push-диагностические данные в рабочей области.](https://go.microsoft.com/fwlink/?linkid=2128284) Диагностические данные из клиента WVD можно вывести в аналитику журналов для своей рабочей области.
1. [Выявлять и диагностировать внутренние](https://go.microsoft.com/fwlink/?linkid=2128338) или внешние проблемы по отношению к WVD.

Дополнительные данные о настройке средства диагностики служб для WVD см. в средстве ["Use Log Analytics for the diagnostics feature".](https://go.microsoft.com/fwlink/?linkid=2128084)

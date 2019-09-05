---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739506"
---
# <a name="how-to-disable-external-groups"></a>Отключение внешних групп

Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании. Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.
  
После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:
  
- Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу ** \> контент и параметры безопасности** в C.

- В разделе **внешняя система обмена сообщениями**выберите **принудительно применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**

- Нажмите кнопку **Сохранить**.

Дополнительную информацию можно узнать [в статье Отключение внешней системы обмена сообщениями в сети Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  
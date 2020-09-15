---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704141"
---
# <a name="how-to-disable-external-groups"></a>Отключение внешних групп

Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании. Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.
  
После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:
  
- Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу **контент и \> Параметры безопасности** в C.

- В разделе **внешняя система обмена сообщениями**выберите **принудительно применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**

- Выберите **Сохранить**.

Дополнительную информацию можно узнать [в статье Отключение внешней системы обмена сообщениями в сети Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  
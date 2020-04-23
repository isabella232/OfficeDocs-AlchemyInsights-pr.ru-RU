---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720781"
---
# <a name="how-to-disable-external-groups"></a>Отключение внешних групп

Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании. Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.
  
После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:
  
- Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу ** \> контент и параметры безопасности** в C.

- В разделе **внешняя система обмена сообщениями**выберите **принудительно применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**

- Нажмите кнопку **Сохранить**.

Дополнительную информацию можно узнать [в статье Отключение внешней системы обмена сообщениями в сети Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  
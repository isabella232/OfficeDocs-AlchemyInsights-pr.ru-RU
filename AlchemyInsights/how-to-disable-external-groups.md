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
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015633"
---
# <a name="how-to-disable-external-groups"></a>Отключение внешних групп

Yammer внешних сообщений применяется Exchange правил транспорта (ETRs), набор активных элементов управления, чтобы предотвратить обмен информацией о компании. Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer, чтобы использовать правило транспорта Exchange для блокировки внешних сообщений.
  
После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы установить применение ETR в Yammer:
  
- Войдите Yammer в качестве проверенного администратора, а Yammer центра администрирования **перейдите** в C **Content and Security Security \> Параметры.**

- В **статье Внешние сообщения** выберите Exchange Online Exchange правила транспорта **(ETRs) в Yammer.**

- Выберите **Сохранить**.

Дополнительные сведения см. [в тексте Отключение](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)внешних сообщений в Yammer сети.
  
---
title: Автоматическая очистка неактивных устройств в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997091"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Автоматическая очистка неактивных устройств в Intune

Intune позволяет администратору настраивать интервал времени 90–270 дней, по окончании которого неактивные устройства удаляются из службы. Это параметр для всей организации, который вступает в силу сразу после активации. Все устройства, которые не были возвращены на сервер Intune в течение периода, превышающего значение параметра, удаляются без возможности восстановления.

**Примечание.** Для этого действия очистки доступны только объекты устройств MDM. Объекты устройств только с EAS исключаются.

Дополнительные сведения об удалении устройства с учетом параметра очистки устройств и его состояния

Параметр: **Удаление устройств после даты последнего возврата: да (указано определенное значение (N) в днях)**

- С учетом значения (N), настроенного для параметра, служба Intune удаляет устройство через указанное количество дней после последнего успешного возврата.

Параметр: **Удаление устройств после даты последнего возврата: нет**

- Устройство удаляется через 180 дней после истечения срока действия его сертификата, если он не был обновлен.

**Примечание.** В обоих случаях устройство должно быть успешно зарегистрировано в Intune. Регистрация выполняется во время первого возврата устройства в службу Intune.

Если устройство успешно подает заявку на регистрацию в Intune, но его не удается зарегистрировать, оно удаляется через 270 дней после подачи заявки. (90 дней, чтобы пометить устройство как отозванное, и еще 180 дней, чтобы удалить запись.)

В настоящее время консоль Intune не включает механизм установки даты окончания срока действия сертификата для указанного устройства.
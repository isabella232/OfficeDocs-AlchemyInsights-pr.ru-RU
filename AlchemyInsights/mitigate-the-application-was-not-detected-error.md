---
title: Устранение ошибки "Приложение не обнаружено"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810496"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Устранение ошибки "Приложение не обнаружено"

Ошибка установки приложения "Приложение не обнаружено после успешной установки", получаемая от Intune, может возникать на всех основных платформах ОС (Windows, iOS и Android).

Наиболее распространенные сценарии возникновения этой ошибки:

- Приложение обновлено за пределами Intune (из стороннего магазина приложений) после первоначального развертывания. Например, некоторые приложения, такие как Google Chrome, могут выполнять автоматическое обновление.
- Пользователь удалил приложение после первоначальной установки.

Чтобы устранить эту проблему, сначала проверьте затронутые устройства, чтобы определить сценарий возникновения ошибки.

- Если приложение обновлено за пределами Intune, развертывание приложения можно настроить на игнорирование версии приложения. Для этого в разделе **Конфигурация приложений > Сведения о приложении** присвойте параметру **Игнорировать версию приложения** значение **Да**.
- Если целью является клиент, может быть уместно развертывание приложения в качестве "обязательного" с обеспечением развертывания последней версии.
- Кроме того, на платформе iOS можно использовать функцию **автоматического обновления** с помощью программы корпоративных закупок Apple, которую можно настроить на автоматическое обновление до новых версий приложений по мере их появления.

Дополнительные сведения об устранении проблем с установкой приложений см. в статье [Устранение проблем с установкой приложений](https://docs.microsoft.com/intune/troubleshoot-app-install).
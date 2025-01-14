---
title: Справка по настройке ночного света для дисплея
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078737"
---
# <a name="help-with-the-night-light-display-setting"></a>Справка по настройке ночного света для дисплея

Дополнительные сведения о настройке ночного света для дисплея см. в разделе [Настройка ночного света для дисплея в Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Если параметры ночного света в настройках неактивны, проверьте драйвер дисплея. 

1. В поле поиска на панели задач введите **Диспетчер устройств**, а затем выберите **Диспетчер устройств** в списке результатов.
1. Разверните **Адаптеры дисплея**. 

К сожалению, функция ночного света будет недоступна, если ваше устройство использует драйвер DisplayLink или базовый драйвер дисплея.

Функция ночного света использует новейшие графические технологии, поэтому вам может потребоваться обновить драйвер дисплея.  

- Проверьте наличие обновлений, перейдя в раздел **Пуск** > **Параметры** > **Обновление и безопасность** > **Центр обновления Windows** > **Проверить наличие обновлений**.  

ИЛИ

- Посетите веб-сайт службы поддержки производителя оборудования, чтобы вручную скачать и установить последние драйверы дисплея.

## <a name="reset-night-light-in-the-registry"></a>Сброс ночного света в реестре

Если обновление драйвера дисплея не помогло решить проблему, возможно, вам потребуется сбросить ночной свет в реестре.  

**Внимание!** Этот способ устранения неполадок рекомендуется только для опытных пользователей. Внесение неправильных изменений в реестр может привести к возникновению серьезных проблем. Для дополнительной защиты сделайте резервную копию реестра, прежде чем вносить в него изменения, чтобы вы могли восстановить его в случае возникновения проблем.

1. В поле поиска введите **regedit**, а затем выберите **Редактор реестра** в результатах поиска.

1. Откройте следующий раздел реестра: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Экспортируйте и затем удалите следующий подраздел:$$windows.data.bluelightreduction.bluelightreductionstate

1. Экспортируйте и затем удалите следующий подраздел:$$windows.data.bluelightreduction.settings

1. Перезапустите Windows и проверьте, доступны ли параметры ночного света.



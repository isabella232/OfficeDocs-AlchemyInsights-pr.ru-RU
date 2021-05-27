---
title: Индикаторы не работают в браузере Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651511"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Индикаторы не работают в браузере Edge

После создания индикатора он не будет поддерживаться в браузере Edge (Smartscreen). Дополнительные сведения см. в разделе [Создание индикаторов для IP, URL-адресов и доменов](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Шаг 1. Убедитесь в следующем:

- подтвердите правильность индикатора (нет опечаток в IP/URL-адресе, задано правильное действие и правильные группы RBAC).
- Учитывая возможную задержку, следует подождать как минимум 2 часа после создания индикатора.
- Подтвердите подключение системы к Microsoft Defender для конечной точки.
- Проверьте способность систем взаимодействовать с облаком.
- Проверьте подключение и доступность Smartscreen, посетив [проверочный сайт](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Шаг 2. Устранение возможной проблемы

- Убедитесь, что клиентский компьютер соответствует требованиям. Дополнительные сведения см. в разделе [Создание индикаторов для IP, URL-адресов и доменов](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Убедитесь, что вы работаете с последней версией браузера Edge. Чтобы узнать какая версия является последней, см. раздел [Как узнать свою версию Microsoft Edge](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Перезапустите браузер Edge.
- Перейдите на сайт, для которого настроен индикатор. Если сайт выглядит не так, как ожидалось, перейдите к шагу 3. 

## <a name="step-3-collect-data"></a>Шаг 3. Сбор данных

- Сбор диагностических данных **MDEClientAnalyzer**. Инструкции см. в разделе [Проблемы с подключением компьютеров в Microsoft Defender для конечной точки](issues-with-onboarding-machines.md).
- Если установка и сбор данных о трассировке Fiddler для вас не затруднительны, см. раздел [Telerik Fiddler](http://www.telerik.com/fiddler).
- Если вам все же необходима помощь, обратитесь в службу поддержки Майкрософт, выбрав значок "Поддержка", расположенный ниже.

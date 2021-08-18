---
title: Правила сокращения направлений атак
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
- "11228"
- "9005470"
ms.openlocfilehash: f7811c15af21d8e7790e6686bb8ba9e5de3659d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319009"
---
# <a name="attack-surface-reduction-rules"></a>Правила сокращения направлений атак

Исключение файлов или папок может значительно снизить защиту, предоставляемую правилами сокращения направлений атак. Файлы, которые были бы заблокированы правилом, могут запускаться, при этом не ведется запись отчетов или событий. Исключение применяется ко всем правилам, допускающим эти исключения.

Исключения для сокращения направлений атак (СНА) используют тот же синтаксис, что и исключения антивирусной программы в Microsoft Defender. Подробные сведения см. в разделе [Настройки и утверждение исключений для проверки антивирусной программой в Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Во избежание проблем просмотрите [распространенные ошибки, которые следует избегать при определении исключений](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Исключения применяются не для всех правил СНА. Чтобы проверить, поддерживает ли правило исключения, см. таблицу [Правила сокращения направлений атак](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Правила сокращения направлений атак

Все зоны, которые могут быть атакованы злоумышленниками для взлома устройств или сетей организации относятся к направлениям атак. Сокращение направлений атак усиливает защиту устройств и сетей организации, давая злоумышленникам меньше шансов на совершение атак. С этим может помочь настройка правил сокращения направлений атак в Microsoft Defender для конечной точки.

Дополнительные сведения см. в статьях:

- [Сопоставление правила СНА GUID с именем](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Требования к правилам СНА:
    - [Windows 10 Pro версии 1709 или более поздней](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Корпоративная версии 1709 или более поздней](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server версии 1803 (Semi-Annual Channel) или более поздней](https://docs.microsoft.com/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Определение правильного исключения для применения

1. Найдите eventID 1121 или 1122 в журнале Microsoft-Windows-Windows Defender/Operational.

1. Вычислите сценарий блокировки и ее контекст, а затем и подтвердите разблокировку сценария.

1. Считайте значение Path в сведениях о событии, определяющем исключение.
    - Настройте исключение максимально строго.
    - При необходимости примените подстановочный символ (например, замените переменную User).

1. Примените исключение согласно потребностям развертывания. Подробные сведения см. в разделе [Настройка правил сокращения направлений атак](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Исключение не соблюдается

1. Определите, допускаются ли исключения для правила. Подробные сведения см. в разделе [Правила сокращения направлений атак](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Просмотрите примененные исключения и выполните проверку опечаток или неправильно интерпретированных подстановочных символов при помощи данных события. Дополнительные сведения см. в разделе[Поддерживаемые типы исключений](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. если влияние правила слишком большое, попробуйте переместить правило (назад) в режим аудита для дальнейшей проверки. Подробные сведения см. в разделе [Работа функций Microsoft Defender для конечной точки в режиме аудита](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Чтобы принять обращение в службу поддержки, соберите необходимые данные и примените следующую команду:
    
   ** MDEClientAnalyzer.cmd -v**

    Дополнительные сведения см. в разделе [Проблемы с подключением компьютеров в Microsoft Defender для конечных точек](issues-with-onboarding-machines.md).

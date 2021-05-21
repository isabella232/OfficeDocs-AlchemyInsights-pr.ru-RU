---
title: Устранение ошибок с удержаниями при обнаружении электронных данных
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583761"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Устранение ошибок с удержаниями при обнаружении электронных данных

Возникли проблемы с удержаниями при обнаружении электронных данных? Вот некоторые рекомендации:

- Проверьте состояние распространения удержания.  Если отображается состояние **Включено (ожидание)** или **Отключено (ожидание)**, дождись завершения распространения удержания.
- Объединяйте обновления удержаний при обнаружении электронных данных в один массовый запрос вместо многократного обновления политики для каждой транзакции.
- Запустите Set-CaseHoldPolicy <policyname> -RetryDistribution в PowerShell Центра безопасности и соответствия требованиям. Подробные сведения см. в статье [Подключение к оболочке PowerShell Центра безопасности и соответствия требованиям](/powershell/exchange/connect-to-scc-powershell).

Инструкции по проверке этих параметров и дополнительные рекомендации по устранению проблем с удержаниями при обнаружении электронных данных см. в статье [Устранение ошибок с удержаниями при обнаружении электронных данных](/microsoft-365/compliance/hold-distribution-errors).
Сведения об устранении других распространенных проблем с обнаружением электронных данных см. в статье [Исследование, устранение неполадок и исправление распространенных проблем с обнаружением электронных данных](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).

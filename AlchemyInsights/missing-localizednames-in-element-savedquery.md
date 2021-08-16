---
title: В элементе 'savedquery' отсутствует 'LocalizedNames'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1739"
- "9000187"
ms.openlocfilehash: 122904b1eb2d1c20fd26bb6a388aa50ced766cec9649fce15c0fae7f6b322832
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065621"
---
# <a name="missing-localizednames-in-element-savedquery"></a>В элементе 'savedquery' отсутствует 'LocalizedNames'

Сведения о действиях в случае отсутствия 'LocalizedNames' см. в статье [При импорте решения Dynamics 365 возникает ошибка "Содержимое элемента 'savedquery' является неполным. Список ожидаемых элементов: 'LocalizedNames'"](https://support.microsoft.com/help/4463330/the-element-savedquery-has-incomplete-content-list-of-possible-element).

Найдите специальные символы в имени представления, которые могут вызывать эту проблему. Удалите все специальные символы в имени представления и выполните экспорт решения повторно.
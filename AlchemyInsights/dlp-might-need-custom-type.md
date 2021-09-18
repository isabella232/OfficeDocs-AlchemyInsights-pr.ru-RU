---
title: DLP может потребоваться настраиваемый тип
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446704"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP может потребоваться настраиваемый тип

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP может требовать настраиваемого типа информации**

Политика предотвращения потери данных (DLP) может определять и защищать конфиденциальные данные в организации. В некоторых сценариях может потребоваться создать собственный настраиваемый тип конфиденциальной информации для защиты данных организации. Дополнительные сведения см. в [дополнительных](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) сведениях о типах конфиденциальной информации и определениях сущности типа [конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Дополнительные сведения о создании настраиваемой конфиденциальной информации типов и политик см. в 

**Настройка встроенных типов конфиденциальной информации**

Если встроенный тип конфиденциальной информации будет отвечать вашим потребностям с помощью нескольких настроек, см. в рубке Настройка встроенного [типа конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Например, можно добавить или удалить ключевые слова или добавить или удалить подтверждающие данные, такие как дата или адрес.

**Создание пользовательского типа конфиденциальных данных**

Но если вам необходимо идентифицировать и защитить конфиденциальные сведения другого типа, можно создать настраиваемый тип конфиденциальной информации в Центр соответствия требованиям Microsoft 365. Дополнительные сведения см. в [ссылке Начало работы с настраиваемыми типами конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Создание пользовательского типа конфиденциальной информации в PowerShell Центра безопасности и соответствия требованиям**

Наконец, если пользовательский интерфейс не предоставляет все необходимые параметры, можно создать настраиваемый тип конфиденциальной информации в центре безопасности & PowerShell. Начиная с XML-файла, можно использовать все доступные параметры. Дополнительные сведения см. в [руб. Создание настраиваемого типа конфиденциальной информации с помощью PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Чтобы сначала протестировать политику в тестовом режиме, см. в таблице [Implement policy in test mode](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) and [Create, test and tune a DLP policy.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 
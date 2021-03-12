---
title: DLP не работает так, как ожидалось
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707823"
---
# <a name="dlp-not-working-as-expected"></a>DLP не работает так, как ожидалось

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Настройка DLP**

У вас возникли проблемы с предотвращением потери данных **(DLP)** в Office 365 не работает, как ожидалось? Если это так, убедитесь, что политика **DLP** настроена правильно и ваши данные содержат то, что ищет политика **DLP** при оценке.
  
Политики DLP позволяют выявлять и защищать конфиденциальные сведения в организации. Чтобы настроить политики DLP, используйте сведения [здесь.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Какие политики DLP**
  
При использовании **встроенных** типов конфиденциальной информации в центрах безопасности и соответствия требованиям политики DLP при обнаружении этих конфиденциальных типов и элементов будут искать определенные шаблоны и элементы.
  
- **Встроенные типы конфиденциальной информации**

    Сведения о встроенных конфиденциальных типах и о том, что ищет политика DLP при обнаружении типа Sensitive, [см.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)в этой таблице.

- **Настраиваемые типы конфиденциальной информации**

    Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого конфиденциального типа: Создание настраиваемого типа [конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Тестирование политики DLP**

Чтобы протестировать данные с помощью встроенного или настраиваемого типа конфиденциальной информации, используйте параметр **Test type** в **типах Classifications**  >  **Sensitive info types.** Дополнительные сведения см. в [специальном тесте типов конфиденциальной информации.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Отчеты**
  
- Получите конфиденциальные сведения о данных с [помощью отчетов DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Дополнительные сведения о событии см. в [отчете об инциденте.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)

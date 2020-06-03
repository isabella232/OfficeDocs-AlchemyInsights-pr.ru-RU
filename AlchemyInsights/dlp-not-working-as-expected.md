---
title: Защита от потери данных не работает должным образом
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507491"
---
# <a name="dlp-not-working-as-expected"></a>Защита от потери данных не работает должным образом

**Важно**. В это беспрецедентное время мы принимаем меры по сохранению высокого уровня доступности служб SharePoint Online и OneDrive. Дополнительные сведения см. в статье [Временные изменения возможностей SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Настройка защиты от потери данных**

Проблемы с **предотвращением потери данных (DLP)** в Office 365 не работают должным образом? Если это так, убедитесь, что **Политика защиты от потери** данных настроена правильно, а данные содержат сведения о том, какую **политику DLP** ищет при оценке.
  
Политики DLP позволяют определять и защищать конфиденциальные данные в Организации. Чтобы настроить политики защиты от потери данных, используйте [здесь](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Поиск в политиках защиты от потери данных**
  
При использовании **встроенных типов конфиденциальных данных** в центрах безопасности и соответствия требованиям политики защиты от потери данных ищут конкретные закономерности и элементы при обнаружении этих конфиденциальных типов.
  
- **Встроенные типы конфиденциальной информации**

    Для получения сведений о встроенных конфиденциальных типах и действиях, выполняемых политикой DLP при определении конфиденциального типа, ознакомьтесь со статьей: [какие типы конфиденциальной информации следует искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Настраиваемые типы конфиденциальной информации**

    Если вы пытаетесь создать настраиваемые типы конфиденциальной информации, используйте следующую статью для получения сведений о создании настраиваемого типа конфиденциальной [информации: Создание настраиваемого типа конфиденциальной информации](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Проверка политики DLP**

Чтобы протестировать данные со встроенным или настраиваемым типом конфиденциальной информации, используйте параметр **тип теста** в разделе **классификация**  >  **типов конфиденциальной**информации. Дополнительные [сведения см.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Отчеты**
  
- Получение конфиденциальных данных с помощью [отчетов о](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports) защите от потери данных.

- Просмотр определенных сведений о событии с [отчетом об инциденте](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).

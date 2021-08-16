---
title: Intune Exchange локального соединиттеля
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013977"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange локального соединиттеля

Подробные сведения о настройке соединитетеля между Intune и Exchange, который находится в локальной среде, см. в следующей документации:

[Настройка локального соединитетеля Intune Exchange в Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Вопросы и ответы:**

В. При попытке настроить соединитетор Exchange я вижу ошибку, например "версия Exchange соединители". В чем может быть причина?

Ответ: Учетная запись, используемая вами, имеет соответствующую лицензию — она должна иметь активную лицензию Intune.

В. Возможно ли иметь несколько соединители Exchange?

О. Можно настроить только один соединитель Exchange для клиента Intune на Exchange организации. Соединитель можно установить только на одном сервере в организации обмена несколькими серверами.

Также нельзя настроить соединители для локального Exchange и Exchange Online в одном клиенте.

В. Может ли соединитатель использовать массив CAS в качестве подключения к Exchange?

О. Указание массива CAS — это не поддерживаемая конфигурация в установке соединитетеля. Только один сервер должен быть указан и должен быть жесткокодирован в файле конфигурации соединитела, который можно найти в

данные программы\Microsoft\Microsoft Intune на локальном Exchange\OnpremiseExchangeConnectorServiceConfiguration.xml

Найдите следующую запись ```<ExchangeWebServiceURL />``` и замените URL-адрес на сервер exchange.

**Пример:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

См. следующую документацию по устранению неполадок: устранение неполадок локального [Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Включение журнала Verbose для соединиттеля Exchange**

1. Откройте файл конфигурации Exchange соединители для редактирования.  
Файл расположен по адресу: %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Пример:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Найдите TraceSourceLine со следующим ключом: OnPremisesExchangeConnectorService  
  
3. Измените значение узла SourceLevel с "Отслеживание информационной активности" (по умолчанию) на "Многословное отслеживание действий"  

**Пример:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Перезапустите службу Microsoft Intune Exchange  
5. Полная синхронизация на портале Intune, пока он не завершится, а затем измените XML на "Отслеживание информационной активности" и перезапустите службу Microsoft Intune Exchange.  
6. Расположение журналов: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`
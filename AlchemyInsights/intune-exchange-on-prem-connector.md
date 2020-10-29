---
title: Локальный соединитель Exchange Intune
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791597"
---
# <a name="intune-exchange-on-premise-connector"></a>Локальный соединитель Exchange Intune

Дополнительные сведения о настройке соединителя между Intune и Exchange, размещенными в локальной среде, можно найти в следующей документации:

[Настройка локального соединителя Exchange Intune в Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Вопросы и ответы:**

В: я вижу сообщение об ошибке "версия Exchange Connector не поддерживается" при попытке настроить соединитель Exchange Connector. Что может быть причиной?

Ответ: используемая учетная запись является лицензированной, она должна иметь активную лицензию Intune

В. можно ли использовать несколько соединителей Exchange?

A: вы можете настроить только один соединитель Exchange Connector для каждого клиента Intune в организации Exchange. Соединитель можно установить только на одном сервере в организации Exchange с несколькими серверами.

Кроме того, вы не можете использовать соединители, настроенные как для локальной среды Exchange, так и для Exchange Online, настроенные в одном клиенте.

Вопрос: может использовать в качестве подключения к Exchange массив CAS?

А: указание массива CAS не поддерживается в настройке соединителя. Необходимо указать только один сервер, который должен быть жестко задан в файле конфигурации соединителя, который можно найти в

Программа дата\микрософт\микрософт Intune на локальном соединителе Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Откройте следующую запись ```<ExchangeWebServiceURL />``` и замените URL-адрес на сервер Exchange.

**Примеры**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Дополнительные сведения об устранении неполадок можно найти в следующей документации: [Устранение неполадок в локальном соединителе Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Включение подробного ведения журнала для соединителя Exchange**

1. Откройте файл конфигурации трассировки Exchange Connector для редактирования.  
Файл находится по адресу:%Програмдата%\микрософт\виндовс Intune Exchange Connector\TracingConfiguration.xml  

**Примеры**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Откройте Трацесаурцелине со следующим ключом: Онпремисесексчанжеконнекторсервице  
  
3. Измените значение узла Саурцелевел с Information АктивититраЦинг (по умолчанию) на Verbose АктивититраЦинг  

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
4. Перезапуск службы Microsoft Intune Exchange  
5. Полную синхронизацию на портале Intune, пока не завершится, а затем замените XML обратно на "Information АктивититраЦинг" и перезапустите службу Microsoft Intune Exchange.  
6. Расположение журналов: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`
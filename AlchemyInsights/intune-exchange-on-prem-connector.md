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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="57001-102">Локальный соединитель Exchange Intune</span><span class="sxs-lookup"><span data-stu-id="57001-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="57001-103">Дополнительные сведения о настройке соединителя между Intune и Exchange, размещенными в локальной среде, можно найти в следующей документации:</span><span class="sxs-lookup"><span data-stu-id="57001-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="57001-104">Настройка локального соединителя Exchange Intune в Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="57001-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="57001-105">**Вопросы и ответы:**</span><span class="sxs-lookup"><span data-stu-id="57001-105">**FAQ:**</span></span>

<span data-ttu-id="57001-106">В: я вижу сообщение об ошибке "версия Exchange Connector не поддерживается" при попытке настроить соединитель Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="57001-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="57001-107">Что может быть причиной?</span><span class="sxs-lookup"><span data-stu-id="57001-107">What could be the cause?</span></span>

<span data-ttu-id="57001-108">Ответ: используемая учетная запись является лицензированной, она должна иметь активную лицензию Intune</span><span class="sxs-lookup"><span data-stu-id="57001-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="57001-109">В. можно ли использовать несколько соединителей Exchange?</span><span class="sxs-lookup"><span data-stu-id="57001-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="57001-110">A: вы можете настроить только один соединитель Exchange Connector для каждого клиента Intune в организации Exchange.</span><span class="sxs-lookup"><span data-stu-id="57001-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="57001-111">Соединитель можно установить только на одном сервере в организации Exchange с несколькими серверами.</span><span class="sxs-lookup"><span data-stu-id="57001-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="57001-112">Кроме того, вы не можете использовать соединители, настроенные как для локальной среды Exchange, так и для Exchange Online, настроенные в одном клиенте.</span><span class="sxs-lookup"><span data-stu-id="57001-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="57001-113">Вопрос: может использовать в качестве подключения к Exchange массив CAS?</span><span class="sxs-lookup"><span data-stu-id="57001-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="57001-114">А: указание массива CAS не поддерживается в настройке соединителя.</span><span class="sxs-lookup"><span data-stu-id="57001-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="57001-115">Необходимо указать только один сервер, который должен быть жестко задан в файле конфигурации соединителя, который можно найти в</span><span class="sxs-lookup"><span data-stu-id="57001-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="57001-116">Программа дата\микрософт\микрософт Intune на локальном соединителе Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="57001-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="57001-117">Откройте следующую запись ```<ExchangeWebServiceURL />``` и замените URL-адрес на сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="57001-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="57001-118">**Примеры**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="57001-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="57001-119">Дополнительные сведения об устранении неполадок можно найти в следующей документации: [Устранение неполадок в локальном соединителе Exchange Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="57001-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="57001-120">**Включение подробного ведения журнала для соединителя Exchange**</span><span class="sxs-lookup"><span data-stu-id="57001-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="57001-121">Откройте файл конфигурации трассировки Exchange Connector для редактирования.</span><span class="sxs-lookup"><span data-stu-id="57001-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="57001-122">Файл находится по адресу:%Програмдата%\микрософт\виндовс Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="57001-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="57001-123">**Примеры**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="57001-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="57001-124">Откройте Трацесаурцелине со следующим ключом: Онпремисесексчанжеконнекторсервице</span><span class="sxs-lookup"><span data-stu-id="57001-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="57001-125">Измените значение узла Саурцелевел с Information АктивититраЦинг (по умолчанию) на Verbose АктивититраЦинг</span><span class="sxs-lookup"><span data-stu-id="57001-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="57001-126">**Пример:**</span><span class="sxs-lookup"><span data-stu-id="57001-126">**Example:**</span></span>
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
4. <span data-ttu-id="57001-127">Перезапуск службы Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="57001-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="57001-128">Полную синхронизацию на портале Intune, пока не завершится, а затем замените XML обратно на "Information АктивититраЦинг" и перезапустите службу Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="57001-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="57001-129">Расположение журналов: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="57001-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>
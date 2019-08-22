---
title: Открытие с помощью проводника не работает
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538497"
---
# <a name="open-with-explorer-isnt-working"></a>Открытие с помощью проводника не работает

Если **окно Открыть в проводнике** или **Просмотреть в проводнике** не работает, убедитесь, что служба WebClient настроена на **Запуск** , выполнив указанные ниже действия. Например, для открытия библиотеки SharePoint или OneDrive может потребоваться много времени, если служба не запущена. 
  
1. В поле поиска Windows введите выполнить, выберите классическое приложение Run. msc, введите Services. msc и нажмите клавишу **Ввод**.
    
2. Прокрутите список вниз до службы WebClient и проверьте столбец **состояние** . Если служба WebClient не **запущена**, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**. Включите службу (при необходимости), выбрав в поле **Тип запуска** значение **вручную** или **автоматически** . 
    
> [!NOTE]
> Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Узнайте, как лучше всего синхронизировать [файлы SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  


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
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419885"
---
# <a name="open-with-explorer-isnt-working"></a>Открытие с помощью проводника не работает

Если **окно Открыть в проводнике** или **Просмотреть в проводнике** не работает, убедитесь, что служба WebClient настроена на **Запуск** , выполнив указанные ниже действия. Например, для открытия библиотеки SharePoint или OneDrive может потребоваться много времени, если служба не запущена. 
  
1. В поле поиска Windows введите выполнить, выберите классическое приложение Run. msc, введите Services. msc и нажмите клавишу **Ввод**.
    
2. ПроКрутите список вниз до службы WebClient и проверьте столбец **состояние** . Если служба WebClient не **запущена**, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**. Включите службу (при необходимости), выбрав в поле **Тип запуска** значение **вручную** или **автоматически** . 
    
> [!NOTE]
> Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Узнайте, как лучше всего синхронизировать [файлы SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  


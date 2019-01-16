---
title: Открыть в проводнике не работает
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307904"
---
# <a name="open-with-explorer-isnt-working"></a>Открыть в проводнике не работает

Если не удается **Открыть в проводнике** или **представления в обозревателе файла** убедитесь, что служба веб-клиента задано значение **под управлением** , выполнив следующие действия. Например он может занять много времени, чтобы открыть библиотеку SharePoint или OneDrive, если служба не запущена. 
  
1. В поле поиска Windows тип запуска, выберите выполнить классического приложения, введите services.msc и выберите **Ввод**.
    
2. Прокрутите список вниз до службу веб-клиента и установить флажок в столбце **состояние** . Если состояние службы веб-клиента не **под управлением**, дважды щелкните имя службы, нажмите кнопку **Пуск**и затем нажмите **кнопку ОК**. Включите службу, при необходимости, выбрав в списке **Тип запуска** **вручную** или **автоматически** . 
    
> [!NOTE]
> Для устранения неполадок, открыв в File Explorer, видеть [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Изучите синхронизации как лучший вариант: [файлы синхронизации SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  


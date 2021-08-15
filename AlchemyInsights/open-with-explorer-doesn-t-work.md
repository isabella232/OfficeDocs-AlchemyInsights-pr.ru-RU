---
title: Open with Explorer не работает
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011349"
---
# <a name="open-with-explorer-isnt-working"></a>Open with Explorer не работает

Если **open with Explorer** или View in File **Explorer** не работает, убедитесь, что служба WebClient настроена на **запуск,** следуя ниже. Например, может потребоваться много времени, чтобы открыть библиотеку SharePoint или OneDrive, когда служба не запущена. 
  
1. В поле Windows введите запуск, выберите настольное приложение Run, введите services.msc и выберите **Ввод**.
    
2. Прокрутите вниз службу WebClient и проверьте **столбец Состояние.** Если состояние службы WebClient не **запущено,** дважды щелкните службу, нажмите кнопку **Начните** и нажмите **кнопку ОК.** Включить службу при необходимости, выбрав  вручную или **автоматический** в поле **типа Запуска.** 
    
> [!NOTE]
> Чтобы устранить проблемы, открываемые в Проводнике файлов, см. [в руб. Open in Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Ознакомьтесь с синхронизацией в качестве лучшей альтернативы: синхронизируйте SharePoint с новым [клиентом приложение синхронизации OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666) 
  


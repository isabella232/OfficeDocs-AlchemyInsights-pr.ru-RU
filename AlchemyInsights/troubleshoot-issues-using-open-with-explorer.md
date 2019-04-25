---
title: Устранение неполадок с помощью команды "открыть в проводнике"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390620"
---
# <a name="fix-problems-with-open-with-explorer"></a>Устранение проблем с открытием в проводнике

Устранение распространенных проблем с открытием библиотеки документов в SharePoint или OneDrive с помощью команды " **Открыть с помощью проводника** ": 
  
- Используйте Internet Explorer 10 или Internet Explorer 11. **Open With Explorer** несовместим с Microsoft EDGE, Google Chrome, Firefox и др. Надстройка " **Открыть в проводнике** " отключена во всех браузерах, кроме Internet Explorer. 
    
- В современном интерфейсе для библиотек SharePoint недоступен режим " **Открыть с помощью проводника** ". Используйте вместо этого **представление в проводнике** . Выберите Просмотр **параметров** \> **в проводнике**. Представление в проводнике не совместимо с Microsoft EDGE, Google Chrome, Firefox и т. д. **Представление в проводнике** доступно только в Internet Explorer. 
    
- Убедитесь, что служба WebClient запущена. В поле поиска Windows введите команду Run (запустить классическое приложение), введите Services. msc и нажмите клавишу ВВОД. ПроКрутите список вниз до службы WebClient и убедитесь, что в столбце **состояние** отображается текст "работает". Если это не так, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**. (Возможно, потребуется сначала включить службу, выбрав в поле **Тип запуска** значение **вручную** или **автоматически** .) 
    
> [!NOTE]
> Открыть библиотеку в проводнике удобно, если вам нужно скопировать или переместить несколько файлов и папок один раз, но если вы хотите регулярно работать в библиотеке, рекомендуем синхронизировать ее. Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Сведения о настройке синхронизации можно найти в статье [Синхронизация файлов SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
В этой статье [описано, как использовать команду "открыть в проводнике" для устранения неполадок в SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) для получения дополнительных сведений. 
  


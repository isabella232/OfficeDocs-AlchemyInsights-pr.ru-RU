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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742746"
---
# <a name="fix-problems-with-open-with-explorer"></a>Устранение проблем с открытием в проводнике

Устранение распространенных проблем с открытием библиотеки документов в SharePoint или OneDrive с помощью команды " **Открыть с помощью проводника** ": 
  
- Используйте Internet Explorer 10 или Internet Explorer 11. **Open With Explorer** несовместим с Microsoft EDGE, Google Chrome, Firefox и др. Надстройка " **Открыть в проводнике** " отключена во всех браузерах, кроме Internet Explorer. 
    
- В современном интерфейсе для библиотек SharePoint недоступен режим " **Открыть с помощью проводника** ". Используйте вместо этого **представление в проводнике** . Выберите Просмотр **параметров** \> **в проводнике**. Представление в проводнике не совместимо с Microsoft EDGE, Google Chrome, Firefox и т. д. **Представление в проводнике** доступно только в Internet Explorer. 
    
- Убедитесь, что служба WebClient запущена. В поле поиска Windows введите команду Run (запустить классическое приложение), введите Services. msc и нажмите клавишу ВВОД. Прокрутите список вниз до службы WebClient и убедитесь, что в столбце **состояние** отображается текст "работает". Если это не так, дважды щелкните службу, нажмите кнопку **Пуск**, а затем нажмите кнопку **ОК**. (Возможно, потребуется сначала включить службу, выбрав в поле **Тип запуска** значение **вручную** или **автоматически** .) 
    
> [!NOTE]
> Открыть библиотеку в проводнике удобно, если вам нужно скопировать или переместить несколько файлов и папок один раз, но если вы хотите регулярно работать в библиотеке, рекомендуем синхронизировать ее. Устранение неполадок, возникающих при открытии в проводнике, представлено в разделе [Открыть в проводнике](https://go.microsoft.com/fwlink/?linkid=871665). Сведения о настройке синхронизации можно найти в статье [Синхронизация файлов SharePoint с помощью нового клиента синхронизации OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
В этой статье [описано, как использовать команду "открыть в проводнике" для устранения неполадок в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) для получения дополнительных сведений. 
  


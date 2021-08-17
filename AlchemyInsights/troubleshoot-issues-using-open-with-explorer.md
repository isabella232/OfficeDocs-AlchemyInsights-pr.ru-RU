---
title: Устранение неполадок с помощью Open with Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048169"
---
# <a name="fix-problems-with-open-with-explorer"></a>Устранение проблем с open with Explorer

Устранение распространенных проблем с открытием библиотеки документов в SharePoint или OneDrive с помощью команды **Open with Explorer:** 
  
- Используйте Internet Explorer 10 или Internet Explorer 11. **Open with Explorer** не совместим с Microsoft Edge, Google Chrome, Firefox и другими. **Open with Explorer** отключен во всех браузерах, кроме Internet Explorer. 
    
- **Open with Explorer** не доступен в современном опыте для SharePoint библиотек. Вместо **этого используйте Представление в обозревателе** файлов. Выберите **параметры** \> **Представления в проводнике файлов.** Просмотр в Проводнике файлов не совместим с Microsoft Edge, Google Chrome, Firefox и другими. **Просмотр в Обозревателе файлов** доступен только в Internet Explorer. 
    
- Убедитесь, что служба WebClient запущена. В поле Windows введите запуск, выберите настольное приложение Run, введите services.msc и нажмите кнопку Ввод. Прокрутите вниз службу WebClient и убедитесь, что столбец **Status** отображает "Запуск". Если этого не сделать, дважды щелкните службу, нажмите **кнопку Начните** и нажмите **кнопку ОК**. (Может потребоваться сначала включить службу,  выбрав вручную или **автоматическую** в поле **типа Запуска.)** 
    
> [!NOTE]
> Открытие библиотеки в Проводнике файлов удобно, если необходимо скопировать или переместить несколько файлов и папок один раз, но если вы хотите регулярно работать в библиотеке, рекомендуется синхронизировать ее. Чтобы устранить проблемы, открываемые в Проводнике файлов, см. [в руб. Open in Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Сведения о настройке синхронизации см. в SharePoint sync с новым [клиентом приложение синхронизации OneDrive.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Дополнительные сведения см. в статье Как использовать команду ["Open with Explorer"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) для устранения неполадок в SharePoint Online. 
  


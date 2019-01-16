---
title: С помощью средства развертывания Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308747"
---
# <a name="using-the-office-deployment-tool-odt"></a>С помощью средства развертывания Office (ODT)

Использовать средство развертывания Office (ODT) для развертывания Office 365 версии Office. Средства развертывания Office (setup.exe), запустите из командной строки и используется XML-файл конфигурации, чтобы определить, какие параметры, применяемые при развертывании Office.
  
1. Загрузите последнюю версию средства развертывания Office из [Центра загрузки Майкрософт](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Использование [Центра развертывания Office (OCT)](https://config.office.com) Выбор параметров развертывания и создать XML-файл конфигурации. Экспорт файла конфигурации и поместите его в ту же папку, где находится программу setup.exe. 
    
    **Примечание:** Адреса файлов конфигурации или проблемы обычно возникают из-за для неправильно настроенный установки Office. Чтобы избежать таких проблем, рекомендуется использовать центр развертывания Office для создания файла конфигурации. Также можно импортировать существующие файлы конфигурации в центр развертывания Office. 
    
3. Из командной строки с повышенными привилегиями перейдите в расположение, где находится setup.exe и запустите средство развертывания Office в режиме загрузки и укажите только что сохраненный файл конфигурации. В следующем примере файла конфигурации с именем Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Запуск средства развертывания Office в режиме configure и указать файл конфигурации.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Примечание:** Это действие необходимо выполнить на клиентском компьютере, на котором необходимо установить Office и необходимо иметь разрешения локального администратора на этом компьютере. 
    
Для получения дополнительных сведений об использовании средства развертывания Office для Office 365 ProPlus сценариев развертывания, просмотрите [Общие сведения о средства развертывания Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Для получения дополнительных сведений о том, как с помощью центра развертывания Office, в разделе [Обзор центра развертывания Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  


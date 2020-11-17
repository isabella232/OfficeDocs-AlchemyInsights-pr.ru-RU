---
title: Использование средства развертывания Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085845"
---
# <a name="using-the-office-deployment-tool-odt"></a>Использование средства развертывания Office (ODT)

Средство развертывания Office (ODT) используется для развертывания версий Office 365 для Office. Средство развертывания Office (setupodt.exe) запускается из командной строки и использует XML-файл конфигурации, чтобы определить, какие параметры следует применить при развертывании Office.
  
1. Скачайте последнюю версию средства развертывания Office в [центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. С помощью [центра развертывания Office (OCT)](https://config.office.com) выберите предпочтения развертывания и создайте XML-файл конфигурации. Экспортируйте файл конфигурации и разместите его локально в той же папке, где находится setupodt.exe.

    **Примечание:** Проблемы с установкой Office обычно возникают из-за неправильной настройки или малформаттед файлов конфигурации. Чтобы избежать подобных проблем, мы рекомендуем использовать центр развертывания Office для создания файла конфигурации. Вы также можете импортировать существующие файлы конфигурации в центр развертывания Office.

3. В командной строки с повышенными привилегиями перейдите в расположение, в котором setupodt.exe размещается и запустите средство развертывания Office в режиме загрузки и укажите только что сохраненный файл конфигурации. В этом примере файл конфигурации имеет имя Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Запустите средство развертывания Office в режиме настройки и укажите файл конфигурации.

```setupodt.exe /configure Configuration.xml```

**Примечание:** Необходимо выполнить это действие с клиентского компьютера, на который необходимо установить Office, и у вас должны быть разрешения локального администратора на этом компьютере.

Чтобы узнать больше об использовании средства развертывания Office для сценариев корпоративного развертывания в приложениях Microsoft 365, ознакомьтесь со статьей [Обзор средства развертывания Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Более подробную информацию об использовании центра развертывания Office можно узнать в статье [Обзор центра развертывания Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

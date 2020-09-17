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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794924"
---
# <a name="using-the-office-deployment-tool-odt"></a>Использование средства развертывания Office (ODT)

Средство развертывания Office (ODT) используется для развертывания версий Office 365 для Office. Средство развертывания Office (setup.exe) запускается из командной строки и использует XML-файл конфигурации, чтобы определить, какие параметры следует применить при развертывании Office.
  
1. Скачайте последнюю версию средства развертывания Office в [центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. С помощью [центра развертывания Office (OCT)](https://config.office.com) выберите предпочтения развертывания и создайте XML-файл конфигурации. Экспортируйте файл конфигурации и разместите его локально в той же папке, где находится setup.exe.

    **Примечание:** Проблемы с установкой Office обычно возникают из-за неправильной настройки или малформаттед файлов конфигурации. Чтобы избежать подобных проблем, мы рекомендуем использовать центр развертывания Office для создания файла конфигурации. Вы также можете импортировать существующие файлы конфигурации в центр развертывания Office.

3. В командной строки с повышенными привилегиями перейдите в расположение, в котором setup.exe размещается и запустите средство развертывания Office в режиме загрузки и укажите только что сохраненный файл конфигурации. В этом примере файл конфигурации имеет имя Configuration.xml:

```setup.exe /download Configuration.xml```

4. Запустите средство развертывания Office в режиме настройки и укажите файл конфигурации.

```setup.exe /configure Configuration.xml```

**Примечание:** Необходимо выполнить это действие с клиентского компьютера, на который необходимо установить Office, и у вас должны быть разрешения локального администратора на этом компьютере.

Чтобы узнать больше об использовании средства развертывания Office для сценариев корпоративного развертывания в приложениях Microsoft 365, ознакомьтесь со статьей [Обзор средства развертывания Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Более подробную информацию об использовании центра развертывания Office можно узнать в статье [Обзор центра развертывания Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).

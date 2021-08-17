---
title: Использование средства Office развертывания
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083783"
---
# <a name="using-the-office-deployment-tool-odt"></a>Использование средства Office развертывания (ODT)

Вы используете Office развертывания (ODT) для развертывания Office 365 версий Office. Средство Office развертывания (setup.exe) запускается из командной строки и использует XML-файл конфигурации, чтобы определить, какие параметры применять при развертывании Office.
  
1. Скачайте последнюю версию средства Office развертывания из [Центра загрузки Майкрософт.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Используйте средство [Office настройки (OCT),](https://config.office.com) чтобы выбрать параметры развертывания и создать XML-файл конфигурации. Экспортировать файл конфигурации и разместить его локально в той же папке, где setup.exe находится.

    **Примечание.** Office часто возникают проблемы с установкой из-за неправильной конфигурации или неправильной формы файлов конфигурации. Чтобы избежать подобных проблем, рекомендуется использовать средство Office настройки для создания файла конфигурации. Вы также можете импортировать существующие файлы конфигурации в Office настройки.

3. Из командной подсказки с повышенными уровнями переключение на расположение, в котором setup.exe, и запустите средство развертывания Office в режиме загрузки и укажите только что сохраненный файл конфигурации. В этом примере файл конфигурации называется Configuration.xml:

```setup.exe /download Configuration.xml```

4. Запустите средство Office развертывания в режиме настройки и укажите файл конфигурации.

```setup.exe /configure Configuration.xml```

**Примечание:** Вы должны выполнить этот шаг с клиентского компьютера, на котором вы хотите установить Office и у вас должны быть локальные разрешения администратора на этом компьютере.

Дополнительные сведения об использовании Office для Приложения Microsoft 365 для предприятий сценариев развертывания см. в обзоре Office [развертывания.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Дополнительные сведения об использовании средства Office настройки см. в обзоре Office [настройки.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)

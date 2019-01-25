---
title: Вопросы об использовании средства развертывания Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486619"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Вопросы об использовании средства развертывания Office (ODT)

Скачайте средство развертывания Office в [ Центре загрузки Майкрософт](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Скачав файл, запустите самоизвлекающийся исполняемый файл, содержащий EXE-файл средства развертывания Office (setup.exe) и пример файла конфигурации (configuration.xml).
  
 **Чтобы исключить или удалить продуктов Office 365 профессиональный плюс с клиентских компьютеров:**
  
При установке Office 365 профессиональный плюс вы можете исключить определенные продукты. Для этого выполните действия по установке Office с помощью средства развертывания Office, но при этом включите элемент ExcludeApp в файл конфигурации. Например, этот файл конфигурации устанавливает все продукты Office 365 профессиональный плюс, кроме Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Общие сведения о средстве развертывания Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


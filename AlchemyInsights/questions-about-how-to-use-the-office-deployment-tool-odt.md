---
title: Вопросы об использовании средства развертывания Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371781"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="b9b18-102">Вопросы об использовании средства развертывания Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="b9b18-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="b9b18-103">Скачайте средство развертывания Office в [ Центре загрузки Майкрософт](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="b9b18-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="b9b18-104">Скачав файл, запустите самоизвлекающийся исполняемый файл, содержащий EXE-файл средства развертывания Office (setup.exe) и пример файла конфигурации (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="b9b18-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="b9b18-105">**Чтобы исключить или удалить продукты Office 365 профессиональный плюс с клиентских компьютеров:**</span><span class="sxs-lookup"><span data-stu-id="b9b18-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="b9b18-p101">При установке Office 365 профессиональный плюс вы можете исключить определенные продукты. Для этого выполните действия по установке Office с помощью средства развертывания Office, но при этом включите элемент ExcludeApp в файл конфигурации. Например, этот файл конфигурации устанавливает все продукты Office 365 профессиональный плюс, кроме Publisher:</span><span class="sxs-lookup"><span data-stu-id="b9b18-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="b9b18-109">Общие сведения о средстве развертывания Office</span><span class="sxs-lookup"><span data-stu-id="b9b18-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  


---
title: Вопросы об использовании средства развертывания Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774904"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="09a0b-102">Вопросы об использовании средства развертывания Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="09a0b-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="09a0b-103">Скачайте средство развертывания Office в [ Центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="09a0b-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="09a0b-104">Скачав файл, запустите самоизвлекающийся исполняемый файл, содержащий EXE-файл средства развертывания Office (setup.exe) и пример файла конфигурации (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="09a0b-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="09a0b-105">**Чтобы исключить или удалить приложения Microsoft 365 для корпоративных продуктов с клиентских компьютеров, выполните указанные ниже действия.**</span><span class="sxs-lookup"><span data-stu-id="09a0b-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="09a0b-106">При установке приложений Microsoft 365 для Enterprise можно исключить определенные продукты.</span><span class="sxs-lookup"><span data-stu-id="09a0b-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="09a0b-107">Для этого выполните действия по установке Office с помощью средства развертывания Office, но при этом включите элемент ExcludeApp в файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="09a0b-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="09a0b-108">Например, в этом файле конфигурации устанавливаются все приложения Microsoft 365 для корпоративных продуктов за исключением издателя:</span><span class="sxs-lookup"><span data-stu-id="09a0b-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="09a0b-109">Общие сведения о средстве развертывания Office</span><span class="sxs-lookup"><span data-stu-id="09a0b-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  


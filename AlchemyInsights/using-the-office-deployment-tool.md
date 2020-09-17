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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="4586a-102">Использование средства развертывания Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="4586a-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="4586a-103">Средство развертывания Office (ODT) используется для развертывания версий Office 365 для Office.</span><span class="sxs-lookup"><span data-stu-id="4586a-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="4586a-104">Средство развертывания Office (setup.exe) запускается из командной строки и использует XML-файл конфигурации, чтобы определить, какие параметры следует применить при развертывании Office.</span><span class="sxs-lookup"><span data-stu-id="4586a-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="4586a-105">Скачайте последнюю версию средства развертывания Office в [центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="4586a-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="4586a-106">С помощью [центра развертывания Office (OCT)](https://config.office.com) выберите предпочтения развертывания и создайте XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4586a-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="4586a-107">Экспортируйте файл конфигурации и разместите его локально в той же папке, где находится setup.exe.</span><span class="sxs-lookup"><span data-stu-id="4586a-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="4586a-108">**Примечание:** Проблемы с установкой Office обычно возникают из-за неправильной настройки или малформаттед файлов конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4586a-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="4586a-109">Чтобы избежать подобных проблем, мы рекомендуем использовать центр развертывания Office для создания файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4586a-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="4586a-110">Вы также можете импортировать существующие файлы конфигурации в центр развертывания Office.</span><span class="sxs-lookup"><span data-stu-id="4586a-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="4586a-111">В командной строки с повышенными привилегиями перейдите в расположение, в котором setup.exe размещается и запустите средство развертывания Office в режиме загрузки и укажите только что сохраненный файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4586a-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="4586a-112">В этом примере файл конфигурации имеет имя Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="4586a-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="4586a-113">4. Запустите средство развертывания Office в режиме настройки и укажите файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4586a-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="4586a-114">**Примечание:** Необходимо выполнить это действие с клиентского компьютера, на который необходимо установить Office, и у вас должны быть разрешения локального администратора на этом компьютере.</span><span class="sxs-lookup"><span data-stu-id="4586a-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="4586a-115">Чтобы узнать больше об использовании средства развертывания Office для сценариев корпоративного развертывания в приложениях Microsoft 365, ознакомьтесь со статьей [Обзор средства развертывания Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="4586a-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="4586a-116">Более подробную информацию об использовании центра развертывания Office можно узнать в статье [Обзор центра развертывания Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="4586a-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>

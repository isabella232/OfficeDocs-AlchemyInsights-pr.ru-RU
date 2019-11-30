---
title: Ошибка активации — мы не можем подключиться прямо сейчас
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628255"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="e690e-102">Устранение неполадок в приложениях Office "сообщение не удается подключиться прямо сейчас"</span><span class="sxs-lookup"><span data-stu-id="e690e-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="e690e-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="e690e-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e690e-104">Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ к приложениям Office через Интернет.</span><span class="sxs-lookup"><span data-stu-id="e690e-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e690e-105">См.: [URL-адреса и диапазоны IP-адресов для Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e690e-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e690e-106">В меню \*\*\*\* > **"** Пуск" выберите команду **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="e690e-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e690e-107">Убедитесь, что запущены следующие службы:</span><span class="sxs-lookup"><span data-stu-id="e690e-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e690e-108">Автоматическая установка подключенных к сети устройств</span><span class="sxs-lookup"><span data-stu-id="e690e-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e690e-109">Служба списка сетей</span><span class="sxs-lookup"><span data-stu-id="e690e-109">Network List Service</span></span>
    - <span data-ttu-id="e690e-110">Служба сетевого расположения</span><span class="sxs-lookup"><span data-stu-id="e690e-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e690e-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="e690e-111">Windows Event Log</span></span>

<span data-ttu-id="e690e-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="e690e-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e690e-113">Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="e690e-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e690e-114">**SFC/Scannow**</span><span class="sxs-lookup"><span data-stu-id="e690e-114">**sfc /scannow**</span></span>

<span data-ttu-id="e690e-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="e690e-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e690e-116">Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "при активации Office из Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e690e-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581888"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="39548-102">Устранение неполадок приложений Microsoft 365 "сообщение о невозможности подключиться прямо сейчас"</span><span class="sxs-lookup"><span data-stu-id="39548-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="39548-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="39548-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="39548-104">Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют Интернет-доступ к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="39548-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="39548-105">См.: [URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="39548-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="39548-106">В меню " **Пуск**" выберите команду  >  **Run** **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="39548-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="39548-107">Убедитесь, что запущены следующие службы:</span><span class="sxs-lookup"><span data-stu-id="39548-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="39548-108">Автоматическая установка подключенных к сети устройств</span><span class="sxs-lookup"><span data-stu-id="39548-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="39548-109">Служба списка сетей</span><span class="sxs-lookup"><span data-stu-id="39548-109">Network List Service</span></span>
    - <span data-ttu-id="39548-110">Служба сетевого расположения</span><span class="sxs-lookup"><span data-stu-id="39548-110">Network Location Awareness</span></span>
    - <span data-ttu-id="39548-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="39548-111">Windows Event Log</span></span>

<span data-ttu-id="39548-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="39548-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="39548-113">Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="39548-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="39548-114">**SFC/Scannow**</span><span class="sxs-lookup"><span data-stu-id="39548-114">**sfc /scannow**</span></span>

<span data-ttu-id="39548-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="39548-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="39548-116">Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "при активации Office из Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="39548-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
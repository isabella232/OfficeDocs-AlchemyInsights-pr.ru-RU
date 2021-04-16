---
title: Проблема активации . Мы не можем подключиться прямо сейчас
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806455"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="3acc7-102">Исправление приложения Microsoft 365 "Мы не можем подключиться прямо сейчас" сообщение</span><span class="sxs-lookup"><span data-stu-id="3acc7-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="3acc7-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="3acc7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3acc7-104">Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не блокируют доступ в Интернет к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3acc7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3acc7-105">См. [диапазоны URL-адресов Microsoft и IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="3acc7-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="3acc7-106">Перейдите **к**  >  **запуску запуска,** а затем **введите services.msc**.</span><span class="sxs-lookup"><span data-stu-id="3acc7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="3acc7-107">Убедитесь, что все следующие службы работают:</span><span class="sxs-lookup"><span data-stu-id="3acc7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="3acc7-108">Автоматическая настройка сетевых подключенных устройств</span><span class="sxs-lookup"><span data-stu-id="3acc7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="3acc7-109">Служба списков сети</span><span class="sxs-lookup"><span data-stu-id="3acc7-109">Network List Service</span></span>
    - <span data-ttu-id="3acc7-110">Осведомленность о расположении сети</span><span class="sxs-lookup"><span data-stu-id="3acc7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="3acc7-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="3acc7-111">Windows Event Log</span></span>

<span data-ttu-id="3acc7-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="3acc7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="3acc7-113">Если у вас возникла проблема с запуском службы, запустите следующую команду, открыв команду с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="3acc7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="3acc7-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="3acc7-114">**sfc /scannow**</span></span>

<span data-ttu-id="3acc7-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="3acc7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="3acc7-116">Подробные сведения см. [в статью "К сожалению, мы не можем подключиться к вашей учетной записи. Попробуйте еще раз" ошибка при активации Office из Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="3acc7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
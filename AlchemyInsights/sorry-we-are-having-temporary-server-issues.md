---
title: Исправление приложений Microsoft 365 К сожалению, у нас есть сообщение о временных проблемах сервера
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835284"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="b71b9-102">Исправление приложения Microsoft 365 "Извините, у нас возникли временные проблемы с сервером"</span><span class="sxs-lookup"><span data-stu-id="b71b9-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="b71b9-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="b71b9-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b71b9-104">Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не блокируют доступ в Интернет к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b71b9-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b71b9-105">См. [url-адреса и диапазоны IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b71b9-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="b71b9-106">Перейдите **к**  >  **запуску запуска,** а затем **введите services.msc**.</span><span class="sxs-lookup"><span data-stu-id="b71b9-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="b71b9-107">Убедитесь, что все следующие службы работают:</span><span class="sxs-lookup"><span data-stu-id="b71b9-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="b71b9-108">Автоматическая настройка сетевых подключенных устройств</span><span class="sxs-lookup"><span data-stu-id="b71b9-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="b71b9-109">Служба списков сети</span><span class="sxs-lookup"><span data-stu-id="b71b9-109">Network List Service</span></span>
    - <span data-ttu-id="b71b9-110">Осведомленность о расположении сети</span><span class="sxs-lookup"><span data-stu-id="b71b9-110">Network Location Awareness</span></span>
    - <span data-ttu-id="b71b9-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="b71b9-111">Windows Event Log</span></span>

<span data-ttu-id="b71b9-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="b71b9-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="b71b9-113">Если у вас возникла проблема с запуском службы, запустите следующую команду, открыв команду с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="b71b9-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="b71b9-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="b71b9-114">**sfc /scannow**</span></span>

<span data-ttu-id="b71b9-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="b71b9-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="b71b9-116">Подробные сведения см. [в статью "К сожалению, мы не можем подключиться к вашей учетной записи. Пожалуйста, попробуйте еще раз" ошибка при активации](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="b71b9-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
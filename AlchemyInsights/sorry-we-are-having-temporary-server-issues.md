---
title: Устранение неполадок в приложениях Office. сообщение о наличии временных проблем с сервером
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764130"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="e9b61-102">Сообщение об исправлении приложений Office "возникли проблемы с временным сервером"</span><span class="sxs-lookup"><span data-stu-id="e9b61-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="e9b61-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="e9b61-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e9b61-104">Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ к приложениям Office через Интернет.</span><span class="sxs-lookup"><span data-stu-id="e9b61-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="e9b61-105">Просмотр [URL-адресов и диапазонов IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e9b61-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="e9b61-106">В меню **Start** > **"** Пуск" выберите команду **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="e9b61-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="e9b61-107">Убедитесь, что запущены следующие службы:</span><span class="sxs-lookup"><span data-stu-id="e9b61-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="e9b61-108">Автоматическая установка подключенных к сети устройств</span><span class="sxs-lookup"><span data-stu-id="e9b61-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="e9b61-109">Служба списка сетей</span><span class="sxs-lookup"><span data-stu-id="e9b61-109">Network List Service</span></span>
    - <span data-ttu-id="e9b61-110">Служба сетевого расположения</span><span class="sxs-lookup"><span data-stu-id="e9b61-110">Network Location Awareness</span></span>
    - <span data-ttu-id="e9b61-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="e9b61-111">Windows Event Log</span></span>

<span data-ttu-id="e9b61-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="e9b61-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="e9b61-113">Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="e9b61-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="e9b61-114">**SFC/Scannow**</span><span class="sxs-lookup"><span data-stu-id="e9b61-114">**sfc /scannow**</span></span>

<span data-ttu-id="e9b61-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="e9b61-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="e9b61-116">Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "ошибка при активации"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="e9b61-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
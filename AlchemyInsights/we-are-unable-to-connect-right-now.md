---
title: Ошибка активации — мы не можем подключиться прямо сейчас
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725996"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="90f90-102">Устранение неполадок приложений Microsoft 365 "сообщение о невозможности подключиться прямо сейчас"</span><span class="sxs-lookup"><span data-stu-id="90f90-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="90f90-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="90f90-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="90f90-104">Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют Интернет-доступ к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="90f90-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="90f90-105">См.: [URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="90f90-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="90f90-106">В меню " **Пуск**" выберите команду  >  **Run** **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="90f90-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="90f90-107">Убедитесь, что запущены следующие службы:</span><span class="sxs-lookup"><span data-stu-id="90f90-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="90f90-108">Автоматическая установка подключенных к сети устройств</span><span class="sxs-lookup"><span data-stu-id="90f90-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="90f90-109">Служба списка сетей</span><span class="sxs-lookup"><span data-stu-id="90f90-109">Network List Service</span></span>
    - <span data-ttu-id="90f90-110">Служба сетевого расположения</span><span class="sxs-lookup"><span data-stu-id="90f90-110">Network Location Awareness</span></span>
    - <span data-ttu-id="90f90-111">Журнал событий Windows</span><span class="sxs-lookup"><span data-stu-id="90f90-111">Windows Event Log</span></span>

<span data-ttu-id="90f90-112">Если одна из этих служб не запущена, попробуйте запустить ее.</span><span class="sxs-lookup"><span data-stu-id="90f90-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="90f90-113">Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:</span><span class="sxs-lookup"><span data-stu-id="90f90-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="90f90-114">**SFC/Scannow**</span><span class="sxs-lookup"><span data-stu-id="90f90-114">**sfc /scannow**</span></span>

<span data-ttu-id="90f90-115">После завершения этой команды перезапустите компьютер.</span><span class="sxs-lookup"><span data-stu-id="90f90-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="90f90-116">Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "при активации Office из Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="90f90-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>
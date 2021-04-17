---
title: Исправление приложений Microsoft 365 Не удалось найти связанное сообщение с лицензиями office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816501"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="2031d-102">Исправление приложения Microsoft 365 "Не удалось найти связанные с лицензиями office" сообщение</span><span class="sxs-lookup"><span data-stu-id="2031d-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="2031d-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="2031d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2031d-104">Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не блокируют доступ в Интернет к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2031d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2031d-105">См. [диапазоны URL-адресов Microsoft 365 и IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2031d-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="2031d-106">Удалите [и перенанаменуем лицензию Office для](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) пострадавшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="2031d-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="2031d-107">Откройте приложение Office и [запишите все](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) существующие учетные записи пользователей.</span><span class="sxs-lookup"><span data-stu-id="2031d-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="2031d-108">Перейдите к настройкам Windows > **учетных записей** электронной почты & учетных записей и удалите все учетные записи, кроме  >  затронутой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2031d-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="2031d-109">Перейдите к параметрам Windows > **работе** или школе доступа к учетным записям и отключите все учетные записи, кроме  >  затронутой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2031d-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="2031d-110">Сбросьте состояние активации Office.</span><span class="sxs-lookup"><span data-stu-id="2031d-110">Reset the Office activation state.</span></span> <span data-ttu-id="2031d-111">[Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="2031d-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="2031d-112">[Во входе](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью учетной записи пострадавшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="2031d-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="2031d-113">Дополнительные решения по устранению неполадок см. в [врезке Unlicensed Product and activation errors in Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="2031d-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
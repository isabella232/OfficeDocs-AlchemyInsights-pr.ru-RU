---
title: Регулирование SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716939"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="6800c-102">Регулирование SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6800c-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="6800c-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">При попытке перейти к сайтам SharePoint или OneDrive пользователи могут получить сообщение о занятости сервера 503.</span></span><span class="sxs-lookup"><span data-stu-id="6800c-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="6800c-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Эта ошибка может быть вызвана регулированием в службе SharePoint. В SharePoint Online используется регулирование, чтобы обеспечить оптимальную производительность и надежность службы SharePoint Online. Регулирование ограничит количество действий пользователей или одновременных вызовов (в соответствии со сценарием или кодом) для предотвращения чрезмерного использования ресурсов. Если вы намерены регулирование, 99% от времени это связано с настраиваемым кодом.</span></span><span class="sxs-lookup"><span data-stu-id="6800c-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="6800c-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Для получения дополнительных сведений об регулированиях см. <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Избегайте регулирования или блокировки в SharePoint Online</a>.</span></span><span class="sxs-lookup"><span data-stu-id="6800c-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="6800c-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Если вы считаете, что эта ошибка не связана с регулированием, вы можете проверить, есть ли активное обслуживание клиента, перейдя в <a href="https://portal.office.com/adminportal/home#/MessageCenter">Центр сообщений</a>. Наконец, убедитесь, что вы посещаете страницу <a href="https://portal.office.com/adminportal/home#/servicehealth">работоспособности службы</a> , чтобы проверить, какие рекомендации и происшествия могут возникать.</span></span><span class="sxs-lookup"><span data-stu-id="6800c-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>



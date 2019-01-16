---
title: Адрес rangesMC146155 1065 амортизации EOP исходящих IP-адресов
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308347"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="a2747-102">Об использовании EOP исходящих диапазоны IP-адресов</span><span class="sxs-lookup"><span data-stu-id="a2747-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="a2747-p101">Обнаружена потенциальная проблема с вашей организации, которые (если не исправленные системой 26 октября 2018) может перестать работать, поток почты в локальной или внешние адреса. Как указывалось ранее для упрощения управления диапазон IP-адресами, мы консолидация выполняется диапазонов адресов Exchange Online Protection (EOP) IP-адресов, которые используются для отправки и получения электронной почты за пределами Office 365. В ходе анализа указывает, что один или несколько источников внешних электронной почты или назначения, которые вы настроили в соединители поток обработки почты не прием подключений от IP-адрес адрес диапазонов показано [здесь](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="a2747-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="a2747-106">Действия перед 26 октября, чтобы убедиться, что эти источники и назначения будет принимать подключений от всех [опубликованных IP-адресов EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="a2747-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="a2747-107">Дополнительные сведения об этом изменении можно найти, центр сообщений учитывает [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="a2747-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="a2747-p102">**Примечание**: Если ранее IP-адрес или URL-адрес публикации с помощью HTML, XML и RSS-канал для обновления конечной точки, также должен миграции на новые веб-служб для автоматизации этих типов обновлений. Для получения дополнительных сведений см [категории конечной точки Office 365 и Office 365 IP-адрес и URL-адрес веб-службы](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="a2747-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  


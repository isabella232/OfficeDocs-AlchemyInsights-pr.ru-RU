---
title: 1065 устаревший исходящий IP-адрес EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858109"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="18453-102">Устаревшие диапазоны исходящих IP-адресов EOP</span><span class="sxs-lookup"><span data-stu-id="18453-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="18453-103">Мы обнаружили потенциальную ошибку в Организации, которая (если она не исправлена в октябре 26th, 2018) может нарушить процесс обработки почты для локальных или внешних назначений.</span><span class="sxs-lookup"><span data-stu-id="18453-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="18453-104">Как было сказано ранее, для упрощения управления диапазоном IP-адресов мы консолидируем диапазоны IP-адресов Exchange Online Protection (EOP), которые используются для отправки и получения электронной почты за пределами Office 365.</span><span class="sxs-lookup"><span data-stu-id="18453-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="18453-105">Наш анализ означает, что один или несколько внешних источников электронной почты или назначений, настроенных в соединителях обработки почты, не принимают подключения из диапазонов IP-адресов, показанных [здесь](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="18453-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="18453-106">Прежде чем Октябрь 26th, убедитесь, что эти источники и назначения будут принимать подключения ко всем [опубликованНЫМ IP-адресАМ EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)и от них.</span><span class="sxs-lookup"><span data-stu-id="18453-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="18453-107">Дополнительные сведения об этом изменении можно найти в центре сообщений posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="18453-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="18453-108">**Note**: Если вы ранее использовали протокол IP или URL-публикацию с помощью HTML, XML и RSS для обновлений конечных точек, вы также должны выполнить миграцию на новые веб-службы для автоматизации этих типов обновлений.</span><span class="sxs-lookup"><span data-stu-id="18453-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="18453-109">Для получения дополнительных сведений см. [категории конечных точек office 365 и IP-адрес office 365 и веб-служба URL-адресов](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="18453-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>

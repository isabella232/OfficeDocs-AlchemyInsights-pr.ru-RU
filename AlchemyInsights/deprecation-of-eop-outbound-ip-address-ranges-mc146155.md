---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031275"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Амортизации исходящие диапазоны IP-адресов EOP

Мы обнаружили потенциальную проблему с вашей организацией, которая (если она не исправлена до 26 октября 2018 г.) может привести к нарушению потока почты в локальном или внешнем назначениях. Как сообщалось ранее, для упрощения управления диапазоном IP-адресов мы консолидировать диапазоны IP Exchange Online Protection (EOP), которые используются для отправки и получения электронной почты за пределами Microsoft 365. Наш анализ показывает, что один или несколько внешних источников электронной почты или назначения, настроенные в соединители потока почты, не принимают подключения из показанных здесь диапазонов [IP-адресов.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Закон до 26 октября, чтобы убедиться, что эти источники и назначения будут принимать подключения к и из всех опубликованных [IP-адресов EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Дополнительные сведения об этом изменении см. в публикации Центра сообщений [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Примечание.** Если вы ранее использовали публикации IP или URL-адресов с помощью HTML, XML и RSS для обновлений конечной точки, необходимо также перейти на новые веб-службы для автоматизации этих типов обновлений. Дополнительные сведения см. в Microsoft 365 категориях конечных точек и [Microsoft 365 IP-адресе и веб-службе URL-адресов.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)

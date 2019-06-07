---
title: 1065 устаревший исходящий IP-адрес EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752968"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Устаревшие диапазоны исходящих IP-адресов EOP

Мы обнаружили потенциальную ошибку в Организации, которая (если она не исправлена в октябре 26th, 2018) может нарушить процесс обработки почты для локальных или внешних назначений. Как было сказано ранее, для упрощения управления диапазоном IP-адресов мы консолидируем диапазоны IP-адресов Exchange Online Protection (EOP), которые используются для отправки и получения электронной почты за пределами Office 365. Наш анализ означает, что один или несколько внешних источников электронной почты или назначений, настроенных в соединителях обработки почты, не принимают подключения из диапазонов IP-адресов, показанных [здесь](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Прежде чем Октябрь 26th, убедитесь, что эти источники и назначения будут принимать подключения ко всем [опубликованным IP-адресам EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)и от них.

Дополнительные сведения об этом изменении можно найти в центре сообщений posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Note**: Если вы ранее использовали протокол IP или URL-публикацию с помощью HTML, XML и RSS для обновлений конечных точек, вы также должны выполнить миграцию на новые веб-службы для автоматизации этих типов обновлений. Для получения дополнительных сведений см. [категории конечных точек office 365 и IP-адрес office 365 и веб-служба URL-адресов](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).

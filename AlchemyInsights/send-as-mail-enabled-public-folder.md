---
title: Отправка общедоступной папки с включенной поддержкой почты в EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451385"
---
# <a name="sendas-mail-enabled-public-folder"></a>Общедоступная папка с включенной поддержкой почты SendAs

В следующем примере назначается разрешение "Отправить как" для общедоступной папки с включенной поддержкой почты NewPF1 пользователю Жасон.

Add-RecipientPermission — Identity "NewPF1" — доверенное лицо "Жасон" — AccessRights "SendAs"

Для получения подробных сведений о синтаксисе и параметрах см. [разрешения "Отправить как" или "Отправить от имени" для общедоступных папок, поддерживающих почту](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).


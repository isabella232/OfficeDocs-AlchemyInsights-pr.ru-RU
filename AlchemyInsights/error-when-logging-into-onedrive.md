---
title: 0x8004de40 при запуске OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813665"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 при запуске OneDrive

Если при входе в OneDrive **0x8004de40** ошибка, перезагружайте компьютер, подключив его к работе или школьному домену. Если вы получили эту ошибку после перезагрузки, попробуйте ее, подключившись к работе или школьному домену:

1. Нажмите кнопку Начните  и введите **командную** команду или командную подсказку в поле поиска, нажмите правой кнопкой мыши на командном запросе и выберите **Выполнить в качестве администратора.** Если вам предложен пароль администратора или подтверждение, введите пароль или нажмите **кнопку Разрешить**.  

2. В окне Командная подсказка введите **dsregcmd/leave**  и дождись завершения команды. Затем **введите dsregcmd/join** и дождитесь завершения команды.
3. Перезагрузка компьютера.

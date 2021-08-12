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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946592"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 при запуске OneDrive

Если при входе **0x8004de40** во время входа OneDrive, перезагружайте компьютер, подключив его к работе или школьному домену. Если вы получили эту ошибку после перезагрузки, попробуйте ее, подключившись к работе или школьному домену:

1. Нажмите кнопку Начните  и введите **командную** команду или командную подсказку в поле поиска, нажмите правой кнопкой мыши на командном запросе и выберите **Выполнить в качестве администратора.** Если вам предложен пароль администратора или подтверждение, введите пароль или нажмите **кнопку Разрешить**.  

2. В окне Командная подсказка введите **dsregcmd/leave**  и дождись завершения команды. Затем **введите dsregcmd/join** и дождитесь завершения команды.
3. Перезагрузка компьютера.

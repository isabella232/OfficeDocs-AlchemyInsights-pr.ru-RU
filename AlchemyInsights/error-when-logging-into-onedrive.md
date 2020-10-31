---
title: Ошибка 0x8004de40 при запуске OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816023"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>Ошибка 0x8004de40 при запуске OneDrive

При получении сообщения об ошибке **0x8004de40** при входе в OneDrive перезагрузите компьютер, подключенный к рабочему или учебному домену. Если после перезагрузки возникает эта ошибка, попробуйте подключиться к рабочему или учебному домену:

1. Нажмите кнопку Пуск и введите в поле поиска **cmd** или **командную строку**  , щелкните правой кнопкой мыши приложение командной строки и выберите  **Запуск от имени администратора** . При получении запроса на ввод пароля администратора или подтверждения введите пароль или нажмите кнопку **Разрешить** .  

2. В окне командной строки введите **дсрегкмд/леаве**  и дождитесь завершения команды. Затем введите **дсрегкмд/Жоин** и дождитесь завершения команды.
3. Перезагрузите компьютер.

---
title: Невозможно получить доступ к файлам, отправленным в чат Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 42731693c062b961bdd3bf7b728ea64f705765e539ee751903dd57f263d11ae0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092453"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a>Невозможно получить доступ к файлам, отправленным в чат Teams

В Microsoft Teams файл, которым пользователь поделился в окне чата, автоматически сохраняется на сайте OneDrive пользователя, предоставляющего общий доступ.

Если другой пользователь пытается открыть файл в Teams и видит сообщение об ошибке "У вас нет доступа к этому файлу", проблема связана с тем, что активирован режим блокировки разрешений пользователей с ограниченным доступом на сайте OneDrive.

1. Инструкции по отключению этой функции на сайте OneDrive см. в статье [Ошибка при открытии файла в Teams](https://go.microsoft.com/fwlink/?linkid=2155733).

1. Проверьте, есть ли у другого пользователя доступ к сайту OneDrive, и предоставьте доступ, следуя инструкциям в статье [Общий доступ к файлам и папкам OneDrive](https://go.microsoft.com/fwlink/?linkid=2156017).
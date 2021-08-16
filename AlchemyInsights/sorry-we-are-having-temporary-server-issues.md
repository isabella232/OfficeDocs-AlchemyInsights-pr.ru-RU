---
title: Исправление Microsoft 365 приложений К сожалению, у нас есть сообщение о временных проблемах сервера
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021609"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Исправление Microsoft 365 приложения "К сожалению, у нас возникли временные проблемы с сервером"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси,чтобы подтвердить, что они не блокируют доступ к Microsoft 365 приложениям. См. [url-адреса и диапазоны IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Перейдите **к**  >  **запуску запуска,** а затем **введите services.msc**. Убедитесь, что все следующие службы работают:
    - Автоматическая настройка сетевых подключенных устройств
    - Служба списков сети
    - Осведомленность о расположении сети
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если у вас возникла проблема с запуском службы, запустите следующую команду, открыв команду с повышенными разрешениями:

**sfc/scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см. [в статью "К сожалению, мы не можем подключиться к вашей учетной записи. Пожалуйста, попробуйте еще раз" ошибка при активации](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
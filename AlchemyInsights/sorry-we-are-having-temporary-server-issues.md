---
title: Исправление приложений Microsoft 365 К сожалению, у нас есть сообщение о временных проблемах сервера
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
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835284"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Исправление приложения Microsoft 365 "Извините, у нас возникли временные проблемы с сервером"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не блокируют доступ в Интернет к приложениям Microsoft 365. См. [url-адреса и диапазоны IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Перейдите **к**  >  **запуску запуска,** а затем **введите services.msc**. Убедитесь, что все следующие службы работают:
    - Автоматическая настройка сетевых подключенных устройств
    - Служба списков сети
    - Осведомленность о расположении сети
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если у вас возникла проблема с запуском службы, запустите следующую команду, открыв команду с повышенными разрешениями:

**sfc/scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см. [в статью "К сожалению, мы не можем подключиться к вашей учетной записи. Пожалуйста, попробуйте еще раз" ошибка при активации](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
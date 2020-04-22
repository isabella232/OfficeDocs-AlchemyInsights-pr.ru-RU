---
title: Устранение неполадок в приложениях Office. сообщение о наличии временных проблем с сервером
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764130"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Сообщение об исправлении приложений Office "возникли проблемы с временным сервером"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ к приложениям Office через Интернет. Просмотр [URL-адресов и диапазонов IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. В меню **Start** > **"** Пуск" выберите команду **Services. msc**. Убедитесь, что запущены следующие службы:
    - Автоматическая установка подключенных к сети устройств
    - Служба списка сетей
    - Служба сетевого расположения
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:

**SFC/Scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "ошибка при активации"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
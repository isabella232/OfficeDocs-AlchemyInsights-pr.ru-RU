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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628003"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Сообщение об исправлении приложений Office "возникли проблемы с временным сервером"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ к приложениям Office через Интернет. См.: [URL-адреса и диапазоны IP-адресов для Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. В меню **** > **"** Пуск" выберите команду **Services. msc**. Убедитесь, что запущены следующие службы:
    - Автоматическая установка подключенных к сети устройств
    - Служба списка сетей
    - Служба сетевого расположения
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:

**SFC/Scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "при активации Office из Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
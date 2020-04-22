---
title: Ошибка активации — мы не можем подключиться прямо сейчас
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716185"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Устранение неполадок в приложениях Office "сообщение не удается подключиться прямо сейчас"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ к приложениям Office через Интернет. См.: [URL-адреса и диапазоны IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. В меню **Start** > **"** Пуск" выберите команду **Services. msc**. Убедитесь, что запущены следующие службы:
    - Автоматическая установка подключенных к сети устройств
    - Служба списка сетей
    - Служба сетевого расположения
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:

**SFC/Scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "при активации Office из Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
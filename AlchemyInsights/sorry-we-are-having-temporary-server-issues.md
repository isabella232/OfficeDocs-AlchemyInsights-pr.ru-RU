---
title: Устранение неполадок приложений Microsoft 365. у нас возникли проблемы с временным сервером
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582716"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Устранение проблемы с приложениями Microsoft 365: сообщение "проблемы с временным сервером"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют Интернет-доступ к приложениям Microsoft 365. Просмотр [URL-адресов и диапазонов IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. В меню " **Пуск**" выберите команду  >  **Run** **Services. msc**. Убедитесь, что запущены следующие службы:
    - Автоматическая установка подключенных к сети устройств
    - Служба списка сетей
    - Служба сетевого расположения
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если при запуске службы возникла проблема, выполните следующую команду, открыв командную строку с повышенными разрешениями:

**SFC/Scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см [. в разделе "Извините, не удается подключиться к вашей учетной записи. Повторите попытку позже "ошибка при активации"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).
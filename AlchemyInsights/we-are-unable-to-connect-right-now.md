---
title: Проблема активации . Мы не можем подключиться прямо сейчас
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744608"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Исправление Microsoft 365 приложения "Мы не можем подключиться прямо сейчас" сообщение

Примечание. Если вы используете более старую версию Windows (например, Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), используйте простое исправление, чтобы включить TLS 1.2 в качестве по умолчанию. Дополнительные сведения см. в статье [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси,чтобы подтвердить, что они не блокируют доступ к Microsoft 365 приложениям. См. [диапазоны URL-адресов Microsoft и IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Перейдите **к**  >  **запуску запуска,** а затем **введите services.msc**. Убедитесь, что все следующие службы работают:
    - Автоматическая настройка сетевых подключенных устройств
    - Служба списков сети
    - Осведомленность о расположении сети
    - Журнал событий Windows

Если одна из этих служб не запущена, попробуйте запустить ее. Если у вас возникла проблема с запуском службы, запустите следующую команду, открыв команду с повышенными разрешениями:

**sfc/scannow**

После завершения этой команды перезапустите компьютер.

Подробные сведения см. [в статью "К сожалению, мы не можем подключиться к вашей учетной записи. Попробуйте еще раз" ошибка](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)при активации Office из Microsoft 365 .
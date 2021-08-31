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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744680"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Исправление Microsoft 365 приложения "К сожалению, у нас возникли временные проблемы с сервером"

Примечание. Если вы используете более старую версию Windows (например, Windows 7 SP1, Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2), используйте простое исправление, чтобы включить TLS 1.2 в качестве по умолчанию. Дополнительные сведения см. в статье [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

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
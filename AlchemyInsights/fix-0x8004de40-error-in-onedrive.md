---
title: Исправление 0x8004de40 ошибки в OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649761"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Исправление 0x8004de40 ошибки в OneDrive

Если вы работаете с Windows 7 и получаете эту ошибку, обновление, чтобы включить [TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)в качестве безопасных протоколов по умолчанию в WinHTTP в Windows .

Если вы работаете с Windows 10 и получаете ошибку 0x8004de40 OneDrive:

- Перезагружайте затронутый компьютер, подключив его к домену Acitve Directory.
- Если перезагрузка не устраняет проблему, отсоединяйтесь и всоедините устройство с Azure AD. 

**Примечание.** Вы должны быть в корпоративной сети при выполнении этих действий. Не выполнять эти действия, если вы не подключены к корпоративной инфраструктуре (например, во время путешествия). 

1. Откройте командную команду с повышенным нажатием, выбрав **команду Начните,** щелкните правой кнопкой **мыши** Командная подсказка, а затем выберите Выполнить в качестве **администратора.**

1. Введите *dsregcmd /leave* and press **Enter**.

1. По завершению введите *dsregcmd/join* и нажмите **кнопку Ввод**.

1. После завершения закроем командную подсказку.

1. Перезагружай компьютер и войдите в OneDrive.
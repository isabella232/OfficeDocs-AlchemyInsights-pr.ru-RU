---
title: Исправление Microsoft 365 приложений не удалось найти связанное сообщение с лицензиями office
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
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069617"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Исправление Microsoft 365 приложения "Не удалось найти связанные лицензии office"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси,чтобы подтвердить, что они не блокируют доступ к Microsoft 365 приложениям. См. [Microsoft 365 URL-адреса и диапазоны IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Удалите [и перенанаменуем лицензию Office для](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) пострадавшего пользователя. 
3. Откройте Приложение Office и [запишите все](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) существующие учетные записи пользователей.
4. Перейдите Windows Параметры > **учетные записи** электронной почты & учетных записей и удалите все учетные записи, за исключением  >  учетной записи, затрагиваемой.
5. Перейдите Windows Параметры > **доступ к** учетным записям и отключите все учетные записи, за исключением  >  затронутой учетной записи.
6. Сбросьте состояние активации Office. [Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Во входе](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью учетной записи пострадавшего пользователя.

Дополнительные решения по устранению неполадок см. в [этой](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)Office.
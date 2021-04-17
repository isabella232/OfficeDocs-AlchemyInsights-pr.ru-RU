---
title: Исправление приложений Microsoft 365 Не удалось найти связанное сообщение с лицензиями office
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816501"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Исправление приложения Microsoft 365 "Не удалось найти связанные с лицензиями office" сообщение

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не блокируют доступ в Интернет к приложениям Microsoft 365. См. [диапазоны URL-адресов Microsoft 365 и IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Удалите [и перенанаменуем лицензию Office для](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) пострадавшего пользователя. 
3. Откройте приложение Office и [запишите все](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) существующие учетные записи пользователей.
4. Перейдите к настройкам Windows > **учетных записей** электронной почты & учетных записей и удалите все учетные записи, кроме  >  затронутой учетной записи.
5. Перейдите к параметрам Windows > **работе** или школе доступа к учетным записям и отключите все учетные записи, кроме  >  затронутой учетной записи.
6. Сбросьте состояние активации Office. [Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Во входе](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью учетной записи пострадавшего пользователя.

Дополнительные решения по устранению неполадок см. в [врезке Unlicensed Product and activation errors in Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
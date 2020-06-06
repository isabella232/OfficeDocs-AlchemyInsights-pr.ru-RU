---
title: При исправлении приложений Microsoft 365, связанных с лицензиями Office, не удалось найти сообщение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580454"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Исправление сообщения о том, что приложение Microsoft 365 "не удалось найти связанные с лицензиями Office"

Если вы получили это сообщение, попробуйте следующее:

1. Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют Интернет-доступ к приложениям Microsoft 365. См.: [URL-адреса и диапазоны IP-адресов Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Удалите и [переназначите лицензию на Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) для соответствующего пользователя. 
3. Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.
4. Откройте раздел Параметры Windows > **учетных**записей & учетных записей  >  **электронной почты**и удалите все рабочие учетные записи, кроме затронутой учетной записи.
5. Перейдите к разделу Параметры Windows > **учетных записей**  >  **работа или учебные**учетные записи и отключите все рабочие учетные записи, кроме затронутой учетной записи
6. Сбросьте состояние активации Office. [Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Выполните вход](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) , используя затронутую учетную запись пользователя.

Дополнительные решения по устранению неполадок приведены [в статье нелицензированные продукты и ошибки активации в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).
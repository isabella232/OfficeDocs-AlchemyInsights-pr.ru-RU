---
title: Проблема активации и входов — сбой в работе доверенного модуля платформы
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
- "3406"
- "9001429"
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822900"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Исправление приложения Microsoft 365 "Модуль доверенных платформ компьютера не функционирует должным образом" сообщение

Чтобы устранить эту ошибку, попробуйте выполнить следующие действия.

1. Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.   
2. С помощью  >  **учетных записей параметров** Windows  >  **& учетные записи,** удалите существующие учетные записи. 
3. С помощью windows **Settings**  >  **Accounts**  >  **Access work or school** отключите существующие учетные записи. 
4. Сбросьте состояние активации Office. [Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)
5. Попробуйте [процесс восстановления пользователей,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) чтобы устранить сбои в работе модуля доверенных платформ (TPM).
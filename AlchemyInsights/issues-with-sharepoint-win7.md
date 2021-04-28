---
title: Проблемы с SharePoint на компьютерах с Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067001"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Проблемы с SharePoint на компьютерах с Windows 7

Если при работе с SharePoint или OneDrive на компьютерах с Windows 7 у вас возникают ошибки, они могут быть связаны с прекращением поддержки TLS 1.0/1.1. Дополнительные сведения:

- [Подготовка к TLS 1.2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- В клиентах Windows 7 SP1 и Windows 8 должен быть включен протокол TLS1.2. Дополнительные сведения см. в статье [Возникновение ошибок проверки подлинности, если у клиента нет поддержки TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Установите KB3140245 и создайте значение реестра. Дополнительные сведения см. в статье  [Обновление для включения TLS 1.1 и TLS 1.2 в качестве стандартных протоколов защиты в WinHTTP в Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- В клиентах Windows 7 SP1 и Windows 8 должны быть установлены последние комплекты шифров TLS. Дополнительные сведения см. в [советах корпорации Майкрософт по безопасности 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 



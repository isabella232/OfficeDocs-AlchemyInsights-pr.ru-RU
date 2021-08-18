---
title: Ретрансляция почты в Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324375"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Настройка многофункционального устройства или приложения для отправки электронной почты

Сведения о вариантах и инструкции см. в статье [Настройка многофункционального устройства или приложения для отправки электронной почты с помощью Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Если у вас есть устройство или приложение, которое недавно перестало работать, наиболее распространенными проблемами являются:

- **Ошибки, связанные с проверкой подлинности при использовании клиента проверки подлинности SMTP**. Мы недавно внесли изменения, связанные с работой проверки подлинности SMTP. Дополнительные сведения об устранении проблем см. в разделе Сбой проверки подлинности в статье [Устранение проблем с принтерами, сканерами и бизнес-приложениями, отправляющими электронную почту с помощью Microsoft 365 или Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Мы поддерживаем только версию TLS 1.2 для обеспечения безопасного подключения к Office 365**. Если вы используете безопасное соединение (TLS), убедитесь, что ваше приложение или устройство поддерживает TLS 1.2. Дополнительные сведения см. в статье [Подготовка к использованию протокола TLS 1.2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Сведения о других проблемах и способах их устранения см. в статье [Устранение проблем с принтерами, сканерами и бизнес-приложениями, отправляющими электронную почту с помощью Microsoft 365 или Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Чтобы просмотреть затронутые устройства, откройте [Отчет о клиентах проверки подлинности SMTP](https://protection.office.com/mailflow/dashboard).

**Примечание**. Exchange Online не поддерживает сценарии массовой рассылки. Чтобы массово рассылать коммерческую электронную почту (например, информационные бюллетени), необходимо использовать сторонних поставщиков, специализирующихся на этих услугах.

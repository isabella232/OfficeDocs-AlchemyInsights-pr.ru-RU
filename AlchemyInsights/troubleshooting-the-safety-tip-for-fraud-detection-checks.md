---
title: Устранение неполадок совет по безопасности проверки обнаружения мошенничества
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955979"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Устранение неполадок совет по безопасности проверки обнаружения мошенничества

Если вы получаете сообщение совет по безопасности в нем говорится: "Отправитель не справился с проверками обнаружения мошенничества и может не быть тем, кем они кажутся", то отправитель не прошел проверки подлинности DKIM или SPF. Самый лучший способ для решения этой проблемы — авторизировать себя. Если отправитель отправляет от вашего имени, необходимо авторизовать его, добавив IP-адрес отправитель в запись SPF.
  
Дополнительные [сведения см. в](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) совет по безопасности устранение неполадок с совет по безопасности проверки обнаружения мошенничества.
  
Вот некоторые другие ссылки, которые могут помочь:
  
- [Как Корпорация Майкрософт использует рамки политики отправитель (SPF) для предотвращения подмены](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настройка SPF для предотвращения спуфинга](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

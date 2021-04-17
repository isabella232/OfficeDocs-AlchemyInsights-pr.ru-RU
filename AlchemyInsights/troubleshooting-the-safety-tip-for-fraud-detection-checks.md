---
title: Устранение неполадок в подсказке безопасности для проверки обнаружения мошенничества
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834744"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Устранение неполадок в подсказке безопасности для проверки обнаружения мошенничества

Если вы получаете подсказку по безопасности с сообщением "Отправитель не справился с проверками обнаружения мошенничества и может не быть тем, кем они кажутся", то отправитель не прошел проверки подлинности DKIM или SPF. Самый лучший способ для решения этой проблемы — авторизировать себя. Если отправитель отправляет от вашего имени, необходимо авторизовать его, добавив IP-адрес отправитель в запись SPF.
  
Дополнительные сведения см. в дополнительных сведениях об устранении неполадок с красным [(подозрительным)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) советом по безопасности для проверки обнаружения мошенничества.
  
Вот некоторые другие ссылки, которые могут помочь:
  
- [Как Корпорация Майкрософт использует рамки политики отправитель (SPF) для предотвращения подмены](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настройка SPF для предотвращения спуфинга](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)

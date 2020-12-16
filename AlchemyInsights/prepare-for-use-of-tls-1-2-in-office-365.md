---
title: Подготовка к использованию протокола TLS 1.2 в Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085917"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Подготовка к использованию протокола TLS 1.2 в Microsoft 365

31 октября 2018 г. будет продолжен переход Microsoft 365 на протокол TLS 1.2. С 15 октября 2020 г. во всей службе O365 начнется процесс отказа от использования TLS 1.0 1.1. Развертывание этого изменения будет осуществляться в течение следующих недель и месяцев, но клиентам следует предполагать, что начиная с 15 октября 2020 г. вызовы по TLS 1.0/1.1 при взаимодействии с O365 работать не будут. Как уже сообщалось (MC126199 в декабре 2017 г., MC128929 в феврале 2018 г., MC186827 в июле 2019 г. и MC218794 в июле 2020 г.), мы переводим все наши веб-службы в режим работы по протоколу TLS 1.2+ по умолчанию, чтобы повысить уровень их безопасности и обеспечить лучшее в своем классе шифрование. Клиенты могут продолжать использовать протоколы TLS 1.0/1.1 для своих серверов и ресурсов, но им следует исходить из предположения о том, что при взаимодействии с ресурсами O365 будет работать только TLS 1.2 или более новые протоколы.
  
Дополнительные сведения об этих изменениях см. в статьях, размещенных [здесь](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) и [здесь](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).

  
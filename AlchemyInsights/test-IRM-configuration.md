---
title: Проверка конфигурации IRM для новых возможностей OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899709"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Проверка конфигурации IRM для новых возможностей OME

Чтобы убедиться, что клиент Microsoft 365 настроен для использования новых возможностей OME, выполните следующие командлеты при подключении к [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell).


1. Проверьте конфигурацию IRM клиента, выполнив `Get-IRMConfiguration`. Установите **True** для этих значений:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Используя свой домен, адрес отправителя и получателя, выполните `Test-IRMConfiguration`. Если проверка не пройдена, изучите свою конфигурацию IRM.

Дополнительные сведения о проверке конфигурации IRM см. в статье [Проверка новой конфигурации OME в Exchange Online PowerShell](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).
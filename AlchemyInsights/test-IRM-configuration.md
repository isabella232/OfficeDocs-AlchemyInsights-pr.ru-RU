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
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908974"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Проверка конфигурации IRM для новых возможностей OME

Чтобы убедиться, что клиент Microsoft 365 настроен для использования новых возможностей OME, выполните следующие командлеты при подключении к [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell).


1. Проверьте конфигурацию IRM клиента, выполнив `Get-IRMConfiguration`. Установите **True** для этих значений:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Используя свой домен, адрес отправителя и получателя, выполните `Test-IRMConfiguration`. Если проверка не пройдена, изучите свою конфигурацию IRM.

Дополнительные сведения о проверке конфигурации IRM см. в статье [Проверка новой конфигурации OME в Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).
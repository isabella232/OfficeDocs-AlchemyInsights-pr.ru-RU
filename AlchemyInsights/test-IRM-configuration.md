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
ms.openlocfilehash: 28267a4cd0aa139467327385b8e85fed1675cf19
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533005"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Проверка конфигурации IRM для новых возможностей OME

Чтобы убедиться, что клиент Microsoft 365 настроен для использования новых возможностей OME, выполните следующие командлеты при подключении к [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell).


1. Проверьте конфигурацию IRM клиента, выполнив `Get-IRMConfiguration`. Установите **True** для этих значений:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Используя свой домен, адрес отправителя и получателя, выполните `Test-IRMConfiguration`. Если проверка не пройдена, изучите свою конфигурацию IRM.

Дополнительные сведения о проверке конфигурации IRM см. в статье [Проверка новой конфигурации OME в Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).
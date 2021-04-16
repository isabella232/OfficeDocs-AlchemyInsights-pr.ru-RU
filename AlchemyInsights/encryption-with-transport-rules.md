---
title: Шифрование с помощью правил транспорта
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813881"
---
# <a name="encryption-with-transport-rules"></a>Шифрование с помощью правил транспорта

В [Центре администрирования Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) вы можете использовать функции шифрования сообщений Office (OME) в правилах потока обработки почты, чтобы активировать шифрование сообщений. Выберите параметр **Применить шифрование сообщений Office 365 и защиту прав** в условии правила транспорта.

- Дополнительные сведения см. в статье [Определение правила потока обработки почты для шифрования](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- В PowerShell используйте командлет [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и присвойте параметру *ApplyOME* значение $true.

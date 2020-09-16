---
title: Шифрование с помощью правил транспорта
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784356"
---
# <a name="encryption-with-transport-rules"></a>Шифрование с помощью правил транспорта

В [Центре администрирования Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) вы можете использовать функции шифрования сообщений Office (OME) в правилах потока обработки почты, чтобы активировать шифрование сообщений. Выберите параметр **Применить шифрование сообщений Office 365 и защиту прав** в условии правила транспорта.

- Дополнительные сведения см. в статье [Определение правила потока обработки почты для шифрования](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- В PowerShell используйте командлет [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и присвойте параметру *ApplyOME* значение $true.

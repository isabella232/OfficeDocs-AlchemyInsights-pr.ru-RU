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
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="211c5-102">Шифрование с помощью правил транспорта</span><span class="sxs-lookup"><span data-stu-id="211c5-102">Encryption with transport rules</span></span>

<span data-ttu-id="211c5-103">В [Центре администрирования Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) вы можете использовать функции шифрования сообщений Office (OME) в правилах потока обработки почты, чтобы активировать шифрование сообщений.</span><span class="sxs-lookup"><span data-stu-id="211c5-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="211c5-104">Выберите параметр **Применить шифрование сообщений Office 365 и защиту прав** в условии правила транспорта.</span><span class="sxs-lookup"><span data-stu-id="211c5-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="211c5-105">Дополнительные сведения см. в статье [Определение правила потока обработки почты для шифрования](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="211c5-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="211c5-106">В PowerShell используйте командлет [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и присвойте параметру *ApplyOME* значение $true.</span><span class="sxs-lookup"><span data-stu-id="211c5-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>

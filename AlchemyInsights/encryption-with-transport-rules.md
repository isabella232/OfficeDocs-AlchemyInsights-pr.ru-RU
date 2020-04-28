---
title: Шифрование с помощью правил транспорта
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915167"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="fd21d-102">Шифрование с помощью правил транспорта</span><span class="sxs-lookup"><span data-stu-id="fd21d-102">Encryption with transport rules</span></span>

<span data-ttu-id="fd21d-103">В [Центре администрирования Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) вы можете использовать функции шифрования сообщений Office (OME) в правилах потока обработки почты, чтобы активировать шифрование сообщений.</span><span class="sxs-lookup"><span data-stu-id="fd21d-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="fd21d-104">Выберите параметр **Применить шифрование сообщений Office 365 и защиту прав** в условии правила транспорта.</span><span class="sxs-lookup"><span data-stu-id="fd21d-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="fd21d-105">Дополнительные сведения см. в статье [Определение правила потока обработки почты для шифрования](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="fd21d-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="fd21d-106">В PowerShell используйте командлет [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и присвойте параметру *ApplyOME* значение $true.</span><span class="sxs-lookup"><span data-stu-id="fd21d-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>

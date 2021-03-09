---
title: Ошибка адресов прокси при создании общего почтового ящика
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568303"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="ca06e-102">Ошибка адресов прокси при создании почтового ящика или другого объекта с включенной электронной почтой</span><span class="sxs-lookup"><span data-stu-id="ca06e-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="ca06e-103">Если вы попытались создать объект с поддержкой электронной почты (почтовый ящик, общий почтовый ящик и т.д.) и получили ошибку "Прокси-адрес "SMTP:alias@domain.com" уже используется...", выбранный вами адрес электронной почты уже взят другим объектом с поддержкой электронной почты в организации.</span><span class="sxs-lookup"><span data-stu-id="ca06e-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="ca06e-104">Необходимо найти пользователя, группу, общий почтовый ящик или общедоступные папки с этим адресом электронной почты и удалить его или изменить адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca06e-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="ca06e-105">Затем можно создать новый объект с включенной электронной почтой с освобожденным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca06e-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="ca06e-106">Чтобы найти его, используйте поиск на домашней странице.</span><span class="sxs-lookup"><span data-stu-id="ca06e-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="ca06e-107">Вы также можете использовать следующую команду Exchange Online PowerShell для поиска:</span><span class="sxs-lookup"><span data-stu-id="ca06e-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="ca06e-108">Если вы не хотите удалять существующий адрес электронной почты, выберите новый адрес электронной почты для нового объекта, который вы создаете.</span><span class="sxs-lookup"><span data-stu-id="ca06e-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  
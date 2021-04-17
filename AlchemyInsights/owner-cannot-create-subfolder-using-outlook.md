---
title: Владелец не может создать вложенную папку с помощью Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836148"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="34ad5-102">Владелец не может создать вложенную папку с помощью Outlook</span><span class="sxs-lookup"><span data-stu-id="34ad5-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="34ad5-103">**Существует проблема с созданием вложенных папок владельцами общедоступных папок с помощью Outlook. Эта проблема будет скоро исправлена.**</span><span class="sxs-lookup"><span data-stu-id="34ad5-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="34ad5-104">Пока же используйте одно из следующих временных решений.</span><span class="sxs-lookup"><span data-stu-id="34ad5-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="34ad5-105">Для создания вложенных папок используйте Outlook для Mac, так как проблема затрагивает только Outlook для классических выпусков Windows (все версии)</span><span class="sxs-lookup"><span data-stu-id="34ad5-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="34ad5-106">Пусть вложенные папки создает администратор с помощью оболочки EXO или EAC</span><span class="sxs-lookup"><span data-stu-id="34ad5-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="34ad5-107">Измените параметр DefaultPublicFolderMailbox/EffectivePublicFolderMailbox пользователя на почтовый ящик, отличный от почтового ящика содержимого, в папке которого возникает проблема</span><span class="sxs-lookup"><span data-stu-id="34ad5-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="34ad5-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="34ad5-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="34ad5-109">Подождите час и перезапустите клиент Outlook</span><span class="sxs-lookup"><span data-stu-id="34ad5-109">Wait for an hour, restart outlook client</span></span>
---
title: Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401449"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="8c471-102">Устранение проблем с доставкой электронной почты для общедоступных папок, поддерживающих почту</span><span class="sxs-lookup"><span data-stu-id="8c471-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="8c471-103">Если внешние отправители не могут отправлять сообщения в общедоступные папки с включенной поддержкой почты, а отправители не могут найти сообщение об ошибке **(550 5.4.1)**, убедитесь, что домен электронной почты для общедоступной папки настроен как домен внутренней ретрансляции, а не в удостоверяющий домен:</span><span class="sxs-lookup"><span data-stu-id="8c471-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="8c471-104">Откройте [центр администрирования Exchange](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8c471-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="8c471-105">Перейдите в раздел **поток** \> обработки почты **обслуживаемые домены**, выберите обслуживаемый домен и нажмите кнопку **изменить**.</span><span class="sxs-lookup"><span data-stu-id="8c471-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="8c471-106">На открывшейся странице "Свойства", если для типа домена задано \*\*\*\* значение "удостоверяющий", измените значение на " **Внутренняя ретрансляция** " и нажмите кнопку **сохранить**.</span><span class="sxs-lookup"><span data-stu-id="8c471-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="8c471-107">Если внешние отправители получают сообщение об ошибке, у **которого нет разрешения (550 5.7.13)**, выполните следующую команду в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , чтобы просмотреть разрешения для анонимных пользователей в общедоступной папке:</span><span class="sxs-lookup"><span data-stu-id="8c471-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="8c471-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Пример: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="8c471-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="8c471-109">Чтобы разрешить внешним пользователям отправлять электронную почту в эту общедоступную папку, добавьте право доступа CreateItems для анонимного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8c471-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="8c471-110">Например, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="8c471-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>

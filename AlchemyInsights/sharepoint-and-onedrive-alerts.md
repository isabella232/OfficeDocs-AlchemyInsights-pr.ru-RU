---
title: Задержки при получении оповещений SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727256"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="73ccc-102">Задержки при получении оповещений SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="73ccc-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="73ccc-103">Сначала проверьте папку нежелательной почты или спама.</span><span class="sxs-lookup"><span data-stu-id="73ccc-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="73ccc-104">Если **задерживается все оповещения из нескольких файлов или библиотек**, перейдите на [панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home?ref=/servicehealth) , чтобы проверить наличие помощников и инцидентов, которые могут возникнуть при работе с SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="73ccc-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="73ccc-105">Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange.</span><span class="sxs-lookup"><span data-stu-id="73ccc-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="73ccc-106">Кроме того, обратите внимание на то, что отправляются другие сообщения электронной почты (если нет), то, скорее всего, есть задержки Exchange.</span><span class="sxs-lookup"><span data-stu-id="73ccc-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="73ccc-107">Если **отдельное оповещение из определенного файла или библиотеки не доставлено**, попытайтесь удалить его и создать повторно.</span><span class="sxs-lookup"><span data-stu-id="73ccc-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="73ccc-108">Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="73ccc-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="73ccc-109">Оповещения не могут быть отправлены в группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="73ccc-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="73ccc-110">Поддерживаются только группы безопасности и O365.</span><span class="sxs-lookup"><span data-stu-id="73ccc-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="73ccc-111">Вы не можете настраивать шаблоны оповещений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="73ccc-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="73ccc-112">Для этого необходимо использовать Microsoft Flow или рабочий процесс SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="73ccc-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>

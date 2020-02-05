---
title: Задержки при получении оповещений SharePoint и OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771228"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="02884-102">Задержки при получении оповещений SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="02884-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="02884-103">Сначала проверьте папку нежелательной почты или спама.</span><span class="sxs-lookup"><span data-stu-id="02884-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="02884-104">Если **задерживается все оповещения из нескольких файлов или библиотек**, перейдите на [панель мониторинга работоспособности службы](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) , чтобы проверить наличие помощников и инцидентов, которые могут возникнуть при работе с SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="02884-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="02884-105">Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange.</span><span class="sxs-lookup"><span data-stu-id="02884-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="02884-106">Кроме того, обратите внимание на то, что отправляются другие сообщения электронной почты (если нет), то, скорее всего, есть задержки Exchange.</span><span class="sxs-lookup"><span data-stu-id="02884-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="02884-107">Если **отдельное оповещение из определенного файла или библиотеки не доставлено**, попытайтесь удалить его и создать повторно.</span><span class="sxs-lookup"><span data-stu-id="02884-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="02884-108">Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="02884-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="02884-109">Оповещения не могут быть отправлены в группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="02884-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="02884-110">Поддерживаются только группы безопасности и O365.</span><span class="sxs-lookup"><span data-stu-id="02884-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="02884-111">Вы не можете настраивать шаблоны оповещений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="02884-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="02884-112">Для этого необходимо использовать Microsoft Flow или рабочий процесс SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="02884-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>

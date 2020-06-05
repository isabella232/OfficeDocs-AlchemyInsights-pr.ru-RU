---
title: Задержки при получении оповещений SharePoint и OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563523"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="ff3bf-102">Задержки при получении оповещений SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="ff3bf-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="ff3bf-103">Сначала проверьте папку нежелательной почты или спама.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="ff3bf-104">Если **задерживается все оповещения из нескольких файлов или библиотек**, перейдите на [панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home?ref=/servicehealth) , чтобы проверить наличие помощников и инцидентов, которые могут возникнуть при работе с SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ff3bf-105">Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ff3bf-106">Кроме того, обратите внимание на то, что отправляются другие сообщения электронной почты (если нет), то, скорее всего, есть задержки Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="ff3bf-107">Если **отдельное оповещение из определенного файла или библиотеки не доставлено**, попытайтесь удалить его и создать повторно.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="ff3bf-108">Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="ff3bf-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="ff3bf-109">Оповещения не могут быть отправлены в группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="ff3bf-110">Поддерживаются только группы безопасности и O365.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="ff3bf-111">Вы не можете настраивать шаблоны оповещений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="ff3bf-112">Для этого необходимо использовать Microsoft Flow или рабочий процесс SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="ff3bf-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>

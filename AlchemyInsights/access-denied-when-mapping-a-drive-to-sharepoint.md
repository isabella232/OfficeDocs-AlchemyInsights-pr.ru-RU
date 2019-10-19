---
title: Отказано в доступе при сопоставлении диска с SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737490"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="9b6bf-102">Устранение проблем с библиотеками SharePoint, сопоставленными с сетевыми дисками</span><span class="sxs-lookup"><span data-stu-id="9b6bf-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="9b6bf-103">При просмотре подключенного сетевого диска может появиться одно из следующих сообщений:</span><span class="sxs-lookup"><span data-stu-id="9b6bf-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="9b6bf-104">**\\Путь недоступен. Возможно, у вас нет разрешения на использование этого сетевого ресурса. Обратитесь к администратору этого сервера, чтобы узнать, есть ли у вас разрешения на доступ.**</span><span class="sxs-lookup"><span data-stu-id="9b6bf-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="9b6bf-105">**Доступ запрещен. Перед открытием файлов в этом расположении необходимо сначала добавить веб-сайт в список надежных сайтов, перейти на веб-сайт и выбрать автоматический вход.**</span><span class="sxs-lookup"><span data-stu-id="9b6bf-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="9b6bf-106">[Справка по устранению неполадок подключенных сетевых дисков](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="9b6bf-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="9b6bf-107">Сопоставление библиотеки как сетевого диска является временным и поддерживается только в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9b6bf-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="9b6bf-108">Вместо этого [синхронизируйте файлы SharePoint с новым клиентом синхронизации OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , который включает [файлы по требованию](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="9b6bf-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="9b6bf-109">Доступ ко всем файлам в OneDrive, не используя локальное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="9b6bf-109">Access all your files in OneDrive without using local storage space.</span></span>
  
---
title: Ошибка входа в OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947504"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="5e2f9-102">Ошибка входа в OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="5e2f9-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="5e2f9-103">При получении сообщения об ошибке "AADSTS50011: URL-адрес ответа, указанный в запросе, не отвечает" при входе в приложение OneDrive, проверьте следующее:</span><span class="sxs-lookup"><span data-stu-id="5e2f9-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="5e2f9-104">Версия OneDrive должна быть больше или равна версии 20.052. XXXX. Означает.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="5e2f9-105">Чтобы проверить версию, щелкните синий значок OneDrive в области уведомлений, выберите **раздел справка & параметры > параметры > о**.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="5e2f9-106">Сеть может блокировать трафик в **g.Live.com** и **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="5e2f9-107">Если этот трафик блокируется, OneDrive не сможет обновить себя.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="5e2f9-108">Свяжитесь с администратором сети, чтобы убедиться, что у вас есть доступ к этим URL-адресам.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="5e2f9-109">[Эти конечные точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) должны быть достижимыми для клиентов, использующих планы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5e2f9-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="5e2f9-110">Если вам нужно получить текущую версию OneDrive вручную, посетите страницу [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="5e2f9-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>

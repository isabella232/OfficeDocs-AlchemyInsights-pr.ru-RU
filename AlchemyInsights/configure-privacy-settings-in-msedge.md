---
title: Настройка параметров конфиденциальности в Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403858"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="b1292-102">Настройка параметров конфиденциальности в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b1292-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="b1292-103">По умолчанию, если Microsoft Edge развернута на платформах, не в windows, диагностические данные и сведения о сайте не отправляются в Корпорацию Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b1292-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="b1292-104">Однако, если Microsoft Edge развернута в Windows 10, диагностические данные и сведения о сайте отправляются в соответствии с настройками диагностических данных [Windows для пользователей.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="b1292-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="b1292-105">Чтобы настроить, как Microsoft Edge обрабатывает сбор данных для организации, используйте следующие групповые политики:</span><span class="sxs-lookup"><span data-stu-id="b1292-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="b1292-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) включает отчеты об использовании и данных, связанных с аварийной аварией.</span><span class="sxs-lookup"><span data-stu-id="b1292-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="b1292-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) отправляет сведения о сайте, используемые для улучшения служб Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b1292-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="b1292-108">Дополнительные новости см. [в перенастройке параметров политики.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="b1292-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>

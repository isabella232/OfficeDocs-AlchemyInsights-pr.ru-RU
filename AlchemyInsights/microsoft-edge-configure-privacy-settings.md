---
title: Microsoft Edge Настройка параметров конфиденциальности
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599515"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="c7382-102">Microsoft Edge Настройка параметров конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="c7382-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="c7382-103">По умолчанию при развертывании Microsoft EDGE на платформах, отличных от Windows, данные диагностики и сведения о сайте не отправляются в корпорацию Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c7382-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="c7382-104">Однако если Microsoft Edge развернут в Windows 10, данные диагностики и сведения о сайте отправляются в соответствии с [параметрами диагностических данных Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7382-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="c7382-105">Чтобы настроить, как Microsoft Edge обрабатывает сбор данных для вашей организации, используйте следующие групповые политики:</span><span class="sxs-lookup"><span data-stu-id="c7382-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="c7382-106">[Метриксрепортинженаблед](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Эта политика позволяет создавать отчеты об использовании и сбоях данных.</span><span class="sxs-lookup"><span data-stu-id="c7382-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="c7382-107">[Сендситеинфотоимпровесервицес](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Эта политика отправляет сведения сайта, используемые для усовершенствования служб Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c7382-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="c7382-108">Чтобы узнать больше, ознакомьтесь со статьей [Настройка параметров политики](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="c7382-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>
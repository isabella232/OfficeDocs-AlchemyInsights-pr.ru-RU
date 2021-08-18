---
title: Microsoft Edge настройки параметров конфиденциальности
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114185"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge настройки параметров конфиденциальности

По умолчанию, Microsoft Edge развертывается на не Windows платформах, диагностические данные и сведения о сайте не отправляются в Корпорацию Майкрософт. Однако если Microsoft Edge развертывается в Windows 10, диагностические данные и сведения о сайте отправляются в соответствии с Windows [параметров диагностических данных.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Чтобы настроить обработку Microsoft Edge для организации, используйте следующие групповые политики:
- [MetricsReportingEnabled.](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Эта политика позволяет сообщать об использовании и данных, связанных с аварийной аварией.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Эта политика отправляет сведения о сайте, которые используются для улучшения службы Майкрософт.

Дополнительные новости см. [в перенастройке параметров политики.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)
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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge Настройка параметров конфиденциальности

По умолчанию при развертывании Microsoft EDGE на платформах, отличных от Windows, данные диагностики и сведения о сайте не отправляются в корпорацию Майкрософт. Однако если Microsoft Edge развернут в Windows 10, данные диагностики и сведения о сайте отправляются в соответствии с [параметрами диагностических данных Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)для пользователей.

Чтобы настроить, как Microsoft Edge обрабатывает сбор данных для вашей организации, используйте следующие групповые политики:
- [Метриксрепортинженаблед](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Эта политика позволяет создавать отчеты об использовании и сбоях данных.
- [Сендситеинфотоимпровесервицес](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Эта политика отправляет сведения сайта, используемые для усовершенствования служб Майкрософт.

Чтобы узнать больше, ознакомьтесь со статьей [Настройка параметров политики](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).
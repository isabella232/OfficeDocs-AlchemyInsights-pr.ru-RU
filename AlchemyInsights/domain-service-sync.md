---
title: Синхронизация службы доменов
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876519"
---
# <a name="domain-service-synchronization"></a>Синхронизация службы доменов

Объекты и учетные данные в управляемом домене доменных служб Azure Active Directory (Azure AD DS) можно создавать локально в домене или синхронизировать с клиентом Azure Active Directory (Azure AD). При первом развертывании Azure AD DS настраивается и инициируется автоматическая синхронизация в одну сторону для репликации объектов из Azure AD. Эта однонаправная синхронизация продолжает работать в фоновом режиме, чтобы поддерживать управляемый домен Azure AD DS в курсе всех изменений, внесенных в Azure AD. Синхронизация из Azure AD DS обратно в Azure AD не происходит.

Дополнительные сведения о синхронизации службы домена Azure Active Directory см. в этой [теме.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 

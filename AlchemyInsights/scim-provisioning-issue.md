---
title: Проблема с подготовкой SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935405"
---
# <a name="scim-provisioning-issue"></a>Проблема с подготовкой SCIM

Понятие "автоматическая подготовка" относится к созданию удостоверений и ролей пользователей в облачных приложениях, к которым пользователям требуется доступ. Помимо создания удостоверений пользователей, автоматическая подготовка включает их обслуживание и удаление при изменении статуса или роли пользователей. Прежде чем запустить развертывание, ознакомьтесь со статьей [Как работает подготовка](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works), чтобы узнать, как работает подготовка Azure Active Directory (AD), и получить рекомендации по конфигурации.

Разработчик приложения может использовать API управления пользователями SCIM (System for Cross-Domain Identity Management) для включения автоматической подготовки пользователей и групп между своим приложением и Azure AD. В статье [Создание конечной точки SCIM и настройка подготовки пользователей в Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) описывается, как создать конечную точку SCIM и интегрировать ее со службой подготовки Azure AD.




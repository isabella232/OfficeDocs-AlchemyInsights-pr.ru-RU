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
# <a name="scim-provisioning-issue"></a><span data-ttu-id="eba1c-102">Проблема с подготовкой SCIM</span><span class="sxs-lookup"><span data-stu-id="eba1c-102">SCIM provisioning issue</span></span>

<span data-ttu-id="eba1c-103">Понятие "автоматическая подготовка" относится к созданию удостоверений и ролей пользователей в облачных приложениях, к которым пользователям требуется доступ.</span><span class="sxs-lookup"><span data-stu-id="eba1c-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="eba1c-104">Помимо создания удостоверений пользователей, автоматическая подготовка включает их обслуживание и удаление при изменении статуса или роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="eba1c-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="eba1c-105">Прежде чем запустить развертывание, ознакомьтесь со статьей [Как работает подготовка](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works), чтобы узнать, как работает подготовка Azure Active Directory (AD), и получить рекомендации по конфигурации.</span><span class="sxs-lookup"><span data-stu-id="eba1c-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="eba1c-106">Разработчик приложения может использовать API управления пользователями SCIM (System for Cross-Domain Identity Management) для включения автоматической подготовки пользователей и групп между своим приложением и Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eba1c-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="eba1c-107">В статье [Создание конечной точки SCIM и настройка подготовки пользователей в Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) описывается, как создать конечную точку SCIM и интегрировать ее со службой подготовки Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eba1c-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>




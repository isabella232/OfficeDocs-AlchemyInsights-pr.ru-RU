---
title: Синхронизация группы
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 7e5ed69c34f8e7b922d7eef202af508152a7e04d7773581b32e43395571c6fbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987660"
---
# <a name="group-sync"></a>Синхронизация группы

В этой статье приведены инструкции по синхронизации групп.

1. Если глобальный администратор или владелец группы не может изменить свойства группы или добавить участников на портале Azure, убедитесь, что главным источником для группы является Azure Active Directory (Azure AD), чтобы глобальный администратор или владелец группы могли изменить группу.
2. Перед удалением синхронизированной группы в Azure AD [удалите все назначенные лицензии](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced), чтобы избежать ошибок.

Сведения о том, как синхронизировать пользователей, группы и контакты, см. в статье [Синхронизация Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), а также в статье [Синхронизация локальной группы с Azure с помощью Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support), чтобы синхронизировать локальные группы с помощью AD Connect.

Чтобы устранить распространенные ошибки во время синхронизации, следуйте инструкциям статьи [Устранение ошибок синхронизации](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors).


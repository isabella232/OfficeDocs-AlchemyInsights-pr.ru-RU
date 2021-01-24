---
title: Сопоставление атрибутов подготовки пользователей
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
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935395"
---
# <a name="user-provisioning-attribute-mapping"></a>Сопоставление атрибутов подготовки пользователей

1. Чтобы устранить известные проблемы при сопоставлении атрибутов, см. статью [Сопоставления атрибутов](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) обеспечивает поддержку подготовки пользователей для сторонних приложений SaaS, таких как Salesforce, G Suite и др. Если включена подготовка пользователей для стороннего приложения SaaS, портал Azure управляет значениями его атрибутов с помощью сопоставлений атрибутов. Сведения о настройке сопоставлений атрибутов по умолчанию см. в статье [Настройка сопоставлений атрибутов подготовки пользователей для приложений SaaS в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Дополнительные сведения о подготовке пользователей приложения SaaS см. в статье [Что такое автоматизированная подготовка пользователей приложения SaaS в Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. При настройке сопоставлений атрибутов для подготовки пользователей может оказаться, что атрибут, который нужно сопоставить, не отображается в списке атрибутов источника. В статье [Синхронизация атрибута из локальной службы Active Directory с Azure AD для подготовки приложения](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) показано, как добавлять отсутствующий атрибут, выполняя его синхронизацию из локальной службы AD с Azure AD.

---
title: Виртуальная настройка с доменными службами AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072857"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Виртуальная настройка с доменными службами AAD

Виртуальная настройка с использованием доменных служб AAD включает следующие действия: 

1. Проверка работоспособности домена на портале Azure https://aka.ms/aadds-health
2. Проверка NSG по поводу правил, которые блокируют порты, необходимые для синхронизации в доменных службах Azure AD, на портале https://aka.ms/aadds-networking
3. Убедитесь, что виртуальная сеть развернута в том же регионе Azure, что и домен, управляемый доменными службами Azure AD.
4. Убедитесь в том, что у вас нет домена с тем же доменным именем, что и в виртуальной сети.

Подробнее о рассмотрении проектирования виртуальной сети Azure для поддержки доменных служб AAD см. в статье [Рассмотрение виртуальной сети](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).


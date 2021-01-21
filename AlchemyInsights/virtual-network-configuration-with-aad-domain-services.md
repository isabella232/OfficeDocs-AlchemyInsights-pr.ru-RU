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
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884612"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Виртуальная настройка с доменными службами AAD

Виртуальная настройка с использованием доменных служб AAD включает следующие действия: 

1. Проверка работоспособности домена на портале Azure https://aka.ms/aadds-health
2. Проверка NSG по поводу правил, которые блокируют порты, необходимые для синхронизации в доменных службах Azure AD, на портале https://aka.ms/aadds-networking
3. Убедитесь, что виртуальная сеть развернута в том же регионе Azure, что и домен, управляемый доменными службами Azure AD.
4. Убедитесь в том, что у вас нет домена с тем же доменным именем, что и в виртуальной сети.

Подробнее о рассмотрении проектирования виртуальной сети Azure для поддержки доменных служб AAD см. в статье [Рассмотрение виртуальной сети](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).


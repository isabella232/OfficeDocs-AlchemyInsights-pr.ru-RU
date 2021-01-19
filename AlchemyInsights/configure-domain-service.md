---
title: Настройка доменных служб
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884621"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Не удается включить AAD-DS или происходит сбой развертывания

Чтобы устранить проблему, при которой доменная служба Azure AD (AAD-DS) не включается или не развертывается, выполните следующие действия:

1. Если используется уже существующая виртуальная сеть, проверьте, нет ли в NSG правил, которые блокируют порты, необходимые для синхронизации в AAD-DS, на портале https://aka.ms/aadds-networking.
2. Проверьте, нет ли ответа о вашем сообщении об ошибке в руководстве по устранению неполадок, которое можно найти в  https://aka.ms/aadds-troubleshoot-enable.
3. Попробуйте выполнить развертывание доменных служб Azure AD в новой виртуальной сети.
4. Следуйте инструкциям в руководстве по началу работы с развертыванием AAD-DS: [Создание и настройка доменных служб AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Если у вас возникли проблемы при развертывании доменных служб Azure AD, см. статью [Устранение неполадок доменных служб Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot), чтобы исправить распространенные ошибки и работать еще эффективнее. 

**Не удалось отключить AAD-DS**

Служба AAD-DS не может быть приостановлена. Чтобы прекратить использование управляемого домена, его нужно удалить.
Сведения об удалении управляемого домена, см. в статье [Удаление доменными службами AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).




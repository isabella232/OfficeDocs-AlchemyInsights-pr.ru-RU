---
title: 'Контроллер домена '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886900"
---
# <a name="domain-controller"></a>Контроллер домена

**Не удается включить AAD-DS или происходит сбой развертывания**

Чтобы устранить проблему, при которой доменная служба Azure AD (AAD-DS) не включается или не развертывается, выполните следующие действия.

1. Если используется уже существующая виртуальная сеть, проверьте, нет ли в NSG правил, которые блокируют порты, необходимые для синхронизации в AAD-DS, на портале https://aka.ms/aadds-networking.
2. Проверьте, нет ли ответа на ваше сообщение об ошибке в руководстве по устранению неполадок, которое можно найти на странице https://aka.ms/aadds-troubleshoot-enable.
3. Попробуйте выполнить развертывание доменных служб Azure AD в новой виртуальной сети.
4. Следуйте инструкциям по началу работы с развертыванием AAD-DS, которые можно найти в [Руководстве по созданию и настройке доменных служб AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Если у вас возникли проблемы при развертывании доменных служб Azure AD, см. статью [Устранение неполадок доменных служб Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot), чтобы исправить распространенные ошибки и работать еще эффективнее. 

**Не удается отключить AAD-DS**

Служба AAD-DS не может быть приостановлена. Чтобы прекратить использование управляемого домена, его нужно удалить.

Сведения по устранению распространенных проблем и восстановлению работоспособности см. в статье [Устранение неполадок доменных служб Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).

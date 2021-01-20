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
# <a name="domain-controller"></a><span data-ttu-id="eb4ea-102">Контроллер домена</span><span class="sxs-lookup"><span data-stu-id="eb4ea-102">Domain controller</span></span>

<span data-ttu-id="eb4ea-103">**Не удается включить AAD-DS или происходит сбой развертывания**</span><span class="sxs-lookup"><span data-stu-id="eb4ea-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="eb4ea-104">Чтобы устранить проблему, при которой доменная служба Azure AD (AAD-DS) не включается или не развертывается, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="eb4ea-105">Если используется уже существующая виртуальная сеть, проверьте, нет ли в NSG правил, которые блокируют порты, необходимые для синхронизации в AAD-DS, на портале https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="eb4ea-106">Проверьте, нет ли ответа на ваше сообщение об ошибке в руководстве по устранению неполадок, которое можно найти на странице https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="eb4ea-107">Попробуйте выполнить развертывание доменных служб Azure AD в новой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="eb4ea-108">Следуйте инструкциям по началу работы с развертыванием AAD-DS, которые можно найти в [Руководстве по созданию и настройке доменных служб AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="eb4ea-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="eb4ea-109">Если у вас возникли проблемы при развертывании доменных служб Azure AD, см. статью [Устранение неполадок доменных служб Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot), чтобы исправить распространенные ошибки и работать еще эффективнее.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="eb4ea-110">**Не удается отключить AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="eb4ea-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="eb4ea-111">Служба AAD-DS не может быть приостановлена.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="eb4ea-112">Чтобы прекратить использование управляемого домена, его нужно удалить.</span><span class="sxs-lookup"><span data-stu-id="eb4ea-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="eb4ea-113">Сведения по устранению распространенных проблем и восстановлению работоспособности см. в статье [Устранение неполадок доменных служб Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="eb4ea-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>

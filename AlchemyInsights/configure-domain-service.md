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
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="3ff7b-102">Не удается включить AAD-DS или происходит сбой развертывания</span><span class="sxs-lookup"><span data-stu-id="3ff7b-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="3ff7b-103">Чтобы устранить проблему, при которой доменная служба Azure AD (AAD-DS) не включается или не развертывается, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="3ff7b-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="3ff7b-104">Если используется уже существующая виртуальная сеть, проверьте, нет ли в NSG правил, которые блокируют порты, необходимые для синхронизации в AAD-DS, на портале https://aka.ms/aadds-networking.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="3ff7b-105">Проверьте, нет ли ответа о вашем сообщении об ошибке в руководстве по устранению неполадок, которое можно найти в  https://aka.ms/aadds-troubleshoot-enable.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="3ff7b-106">Попробуйте выполнить развертывание доменных служб Azure AD в новой виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="3ff7b-107">Следуйте инструкциям в руководстве по началу работы с развертыванием AAD-DS: [Создание и настройка доменных служб AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="3ff7b-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="3ff7b-108">Если у вас возникли проблемы при развертывании доменных служб Azure AD, см. статью [Устранение неполадок доменных служб Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot), чтобы исправить распространенные ошибки и работать еще эффективнее.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="3ff7b-109">**Не удалось отключить AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="3ff7b-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="3ff7b-110">Служба AAD-DS не может быть приостановлена.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="3ff7b-111">Чтобы прекратить использование управляемого домена, его нужно удалить.</span><span class="sxs-lookup"><span data-stu-id="3ff7b-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="3ff7b-112">Сведения об удалении управляемого домена, см. в статье [Удаление доменными службами AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="3ff7b-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>




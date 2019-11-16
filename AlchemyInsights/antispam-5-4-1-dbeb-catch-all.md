---
title: Защиты от спама 5.4.1 DBEB Catch — All
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672446"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="4d305-102">Устранение проблем с доставкой для ошибки с кодом 550 5.4.1 отказ в доступе к ретрансляции</span><span class="sxs-lookup"><span data-stu-id="4d305-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="4d305-103">Эта проблема возникает в тех случаях, когда [проверяется допустимость адреса электронной почты для предотвращения баунцебаккс](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) при входе в сеть Office 365.</span><span class="sxs-lookup"><span data-stu-id="4d305-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="4d305-104">Попробуйте выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="4d305-104">Try the following:</span></span>

1. <span data-ttu-id="4d305-105">Определите, относится ли проблема к целому домену или к одному адресу электронной почты:</span><span class="sxs-lookup"><span data-stu-id="4d305-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="4d305-106">Весь домен: иногда требуется синхронизация домена; Попробуйте [присвоить домену значение Internal, а затем обратно в значение заслуживающий доверия](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="4d305-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="4d305-107">Один адрес электронной почты: иногда необходимо синхронизировать адрес; изменение SMTP-адреса прокси-сервера и его изменение обратно может помочь.</span><span class="sxs-lookup"><span data-stu-id="4d305-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="4d305-108">Определите, характерна ли проблема для группы или общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="4d305-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="4d305-109">Для некоторых типов объектов может потребоваться вручную создать объекты в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4d305-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="4d305-110">Если вам нужна дополнительная помощь, откройте билет поддержки и укажите область ее действия (инклудиднг тип объекта, на который вы отправляетесь), чтобы мы могли помочь вам лучше.</span><span class="sxs-lookup"><span data-stu-id="4d305-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>
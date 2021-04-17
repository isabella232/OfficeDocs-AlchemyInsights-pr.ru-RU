---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821460"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="70a13-102">Устранение проблем с доставкой для кода ошибки 550 5.4.1 Отказ в ретрансляторе доступа</span><span class="sxs-lookup"><span data-stu-id="70a13-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="70a13-103">Эта проблема возникает при [проверке](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) допустимого адреса электронной почты для предотвращения отскоков при входе в сеть Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="70a13-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="70a13-104">Попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="70a13-104">Try the following:</span></span>

1. <span data-ttu-id="70a13-105">Определите, является ли проблема конкретной для всего домена или одного адреса электронной почты:</span><span class="sxs-lookup"><span data-stu-id="70a13-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="70a13-106">Весь домен. Иногда необходимо синхронизировать домен; попробуйте [установить домен на Внутренний, а затем вернуться к авторитетному](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="70a13-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="70a13-107">Единый адрес электронной почты. Иногда требуется синхронизировать адрес; изменение прокси-адреса smtp и его обратное изменение может помочь.</span><span class="sxs-lookup"><span data-stu-id="70a13-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="70a13-108">Определите, является ли проблема конкретной для группы или общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="70a13-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="70a13-109">Для некоторых типов объектов может потребоваться вручную создавать объекты в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70a13-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="70a13-110">Если вам нужна дополнительная помощь, откройте билет поддержки и укажите область проблемы (в том числе тип объекта, в который вы отправляете), чтобы мы могли помочь вам лучше.</span><span class="sxs-lookup"><span data-stu-id="70a13-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>
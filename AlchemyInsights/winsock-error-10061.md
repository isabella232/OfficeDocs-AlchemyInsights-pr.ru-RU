---
title: 1554 Winsock Error 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419993"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="d2dcf-102">Ошибка Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="d2dcf-102">Winsock error 10061</span></span>

<span data-ttu-id="d2dcf-103">Этот код ошибки означает, что Office 365 не удалось установить TCP-сокет (подключение) к конечному узлу.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="d2dcf-104">Наиболее вероятная причина этой ошибки — проблема с настройкой брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="d2dcf-105">Чтобы устранить эту проблему, проверьте указанные ниже параметры.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="d2dcf-106">Проверьте конфигурацию брандмауэра, указав сведения в [диапазонАх адресов и IP-адресов Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) .</span><span class="sxs-lookup"><span data-stu-id="d2dcf-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="d2dcf-107">Если сообщение об ошибке относится только к Exchange Online Protection (EOP), вы уже получали уведомление об изменении [IP-адресов Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d2dcf-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="d2dcf-108">Убедитесь, что ваш поставщик услуг Интернета (ISP) не блокирует порт.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="d2dcf-109">Проверьте параметры промежуточного узла и целевого сервера в соединителях.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="d2dcf-110">Обратите внимание, что Office 365 не блокирует *Входящие* подключения таким образом.</span><span class="sxs-lookup"><span data-stu-id="d2dcf-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>

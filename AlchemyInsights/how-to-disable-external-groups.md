---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720781"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="2e2b1-102">Отключение внешних групп</span><span class="sxs-lookup"><span data-stu-id="2e2b1-102">How to disable External Groups</span></span>

<span data-ttu-id="2e2b1-103">Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании.</span><span class="sxs-lookup"><span data-stu-id="2e2b1-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="2e2b1-104">Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.</span><span class="sxs-lookup"><span data-stu-id="2e2b1-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="2e2b1-105">После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:</span><span class="sxs-lookup"><span data-stu-id="2e2b1-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="2e2b1-106">Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу \*\* \> контент и параметры безопасности\*\* в C.</span><span class="sxs-lookup"><span data-stu-id="2e2b1-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="2e2b1-107">В разделе **внешняя система обмена сообщениями**выберите **принудительно применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="2e2b1-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="2e2b1-108">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="2e2b1-108">Choose **Save**.</span></span>

<span data-ttu-id="2e2b1-109">Дополнительную информацию можно узнать [в статье Отключение внешней системы обмена сообщениями в сети Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="2e2b1-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  
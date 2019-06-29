---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384838"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="fae7d-102">Отключение внешних групп</span><span class="sxs-lookup"><span data-stu-id="fae7d-102">How to disable External Groups</span></span>

<span data-ttu-id="fae7d-103">Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании.</span><span class="sxs-lookup"><span data-stu-id="fae7d-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="fae7d-104">Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fae7d-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="fae7d-105">После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:</span><span class="sxs-lookup"><span data-stu-id="fae7d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="fae7d-106">Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу \*\* \> контент и параметры безопасности\*\* в C.</span><span class="sxs-lookup"><span data-stu-id="fae7d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="fae7d-107">В разделе **внешняя система обмена сообщениями**выберите принудительно **Применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="fae7d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="fae7d-108">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="fae7d-108">Choose **Save**.</span></span>

<span data-ttu-id="fae7d-109">Дополнительные сведения см. [Управление внешним обменом сообщениями в сети Yammer с помощью правил транспорта Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="fae7d-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  
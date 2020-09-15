---
title: Отключение внешних групп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704141"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="edc41-102">Отключение внешних групп</span><span class="sxs-lookup"><span data-stu-id="edc41-102">How to disable External Groups</span></span>

<span data-ttu-id="edc41-103">Служба внешнего обмена сообщениями Yammer применяет правила транспорта Exchange (ETR), набор профилактическых элементов управления для предотвращения предоставления общего доступа к информации о компании.</span><span class="sxs-lookup"><span data-stu-id="edc41-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="edc41-104">Чтобы запретить пользователям создавать внешние группы, необходимо настроить правило транспорта Exchange (ETR), а затем настроить Yammer на использование правила транспорта Exchange, чтобы заблокировать внешний обмен сообщениями.</span><span class="sxs-lookup"><span data-stu-id="edc41-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="edc41-105">После создания правила в центре администрирования Exchange Online выполните следующие действия, чтобы настроить ETR для применения в Yammer:</span><span class="sxs-lookup"><span data-stu-id="edc41-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="edc41-106">Войдите в Yammer как проверенный администратор и в **центре администрирования Yammer**перейдите на страницу **контент и \> Параметры безопасности** в C.</span><span class="sxs-lookup"><span data-stu-id="edc41-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="edc41-107">В разделе **внешняя система обмена сообщениями**выберите **принудительно применить правила транспорта Exchange Online Exchange (ETR) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="edc41-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="edc41-108">Выберите **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="edc41-108">Choose **Save**.</span></span>

<span data-ttu-id="edc41-109">Дополнительную информацию можно узнать [в статье Отключение внешней системы обмена сообщениями в сети Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="edc41-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  
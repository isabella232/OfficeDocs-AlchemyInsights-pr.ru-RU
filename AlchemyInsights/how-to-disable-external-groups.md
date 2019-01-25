---
title: Как отключить внешних групп
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486810"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="8ec14-102">Как отключить внешних групп</span><span class="sxs-lookup"><span data-stu-id="8ec14-102">How to disable External Groups</span></span>

<span data-ttu-id="8ec14-p101">Yammer, внешние системы обмена сообщениями, относятся правила транспорта Exchange (ETRs) набор упреждающего элементов управления для предотвращения сведения о компании из общего доступа. Чтобы запретить пользователям Создание внешних групп, необходимо настроить правило транспорта Exchange (ETR), а затем настройте Yammer использовать правила транспорта Exchange для блокирования внешние системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="8ec14-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="8ec14-105">После создания правила в Exchange Online центра администрирования выполните следующие действия, чтобы задать ETR для применения в Yammer.</span><span class="sxs-lookup"><span data-stu-id="8ec14-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="8ec14-106">Выполните вход в Yammer подтвержденным администратором и в **Yammer центра администрирования**, перейдите к C **контента и безопасность \> параметров безопасности.**</span><span class="sxs-lookup"><span data-stu-id="8ec14-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="8ec14-107">В разделе **Внешние системы обмена сообщениями**, выберите **применения правил транспорта Exchange Exchange Online (ETRs) в сети Yammer.**</span><span class="sxs-lookup"><span data-stu-id="8ec14-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="8ec14-108">Нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="8ec14-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="8ec14-109">Для получения дополнительных сведений см. [Управление внешней системой обмена сообщениями в сети Yammer с помощью правил транспорта Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="8ec14-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  


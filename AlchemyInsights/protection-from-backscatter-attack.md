---
title: Защита от атаки через подложное уведомление о недоставленном сообщении
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898023"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="7f8fc-102">Защита от атаки через подложное уведомление о недоставленном сообщении</span><span class="sxs-lookup"><span data-stu-id="7f8fc-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="7f8fc-103">Backscatter — это подложные уведомления о недоставке (также известные как отчеты о недоставке или сообщения о возврате), присланные вам относительно сообщений, которые вы на самом деле не отправляли.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="7f8fc-104">Спамеры подделывают (так называемый спуфинг) поле **От:** своих сообщений, и часто используют реальные адреса электронной почты, чтобы вызвать доверие к своим сообщениям.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="7f8fc-105">Таким образом, когда отправители нежелательной почты отправляют сообщения несуществующим получателям, почтовый сервер назначения по сути обманом возвращает недоставленное сообщение как часть отчета о недоставке тому, кто его на самом деле не отправлял, но чей адрес указан в поле **От:**.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="7f8fc-106">Дополнительные сведения см. в статье [Подложное уведомление о недоставленном сообщении в EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="7f8fc-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="7f8fc-107">**Защита от подложных уведомлений о недоставленных сообщениях**</span><span class="sxs-lookup"><span data-stu-id="7f8fc-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="7f8fc-108">Чтобы включить защиту от подложных уведомлений о недоставленном сообщении, выполните следующие шаги.</span><span class="sxs-lookup"><span data-stu-id="7f8fc-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="7f8fc-109">**protection.office.com > Управление угрозами > Политика > Антиспам > Выберите политику фильтрации нежелательной почты и политику редактирования > Свойства нежелательной почты > Пометить как спам > Подложные уведомления о недоставленном сообщении > Установите значение "Вкл"**</span><span class="sxs-lookup"><span data-stu-id="7f8fc-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="7f8fc-110">Если вы считаете, что учетная запись была взломана, см. следующие статьи:</span><span class="sxs-lookup"><span data-stu-id="7f8fc-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="7f8fc-111">Реагирование на взлом учетной записи электронной почты</span><span class="sxs-lookup"><span data-stu-id="7f8fc-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="7f8fc-112">Удаление заблокированных пользователей с портала пользователей с ограниченным доступом в Office 365</span><span class="sxs-lookup"><span data-stu-id="7f8fc-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)




---
title: Значок календаря не отображается в клиенте Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576621"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="abad3-102">Значок календаря не отображается в клиенте Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="abad3-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="abad3-103">Для работы с вкладкой **Календарь** в Teams требуется доступ к почтовому ящику Exchange через веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="abad3-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="abad3-104">Почтовый ящик Exchange может быть подключен к сети или локальной среде.</span><span class="sxs-lookup"><span data-stu-id="abad3-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="abad3-105">Для пользователей Online, которые не видят вкладку **Календарь** , убедитесь, что они [лицензированы для почтового ящика Exchange Online, а почтовый ящик включен](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="abad3-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="abad3-106">Если пользователи размещены в локальной среде, необходимо подтвердить работоспособность гибридной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="abad3-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="abad3-107">Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="abad3-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="abad3-108">Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="abad3-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="abad3-109">Дополнительные сведения и инструкции по устранению неполадок приведены в разделе [Устранение неполадок взаимодействия Microsoft Teams и Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="abad3-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>

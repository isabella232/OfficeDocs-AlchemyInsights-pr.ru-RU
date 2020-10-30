---
title: Устранение неполадок в защитнике Microsoft для Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801456"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="e6877-102">Устранение неполадок в защитнике Microsoft для Office 365</span><span class="sxs-lookup"><span data-stu-id="e6877-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="e6877-103">Вы заметили задержки при доставке сообщений?</span><span class="sxs-lookup"><span data-stu-id="e6877-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="e6877-104">Используйте параметр [динамической доставки](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) в политике безопасных вложений ATP.</span><span class="sxs-lookup"><span data-stu-id="e6877-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="e6877-105">Это позволит избежать задержки сообщений при защите получателей от вредоносных файлов.</span><span class="sxs-lookup"><span data-stu-id="e6877-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="e6877-106">Хотите ли вы сообщить о ложных срабатываниях или ложных негативах в корпорацию Майкрософт?</span><span class="sxs-lookup"><span data-stu-id="e6877-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="e6877-107">Используйте эту [ссылку](https://www.microsoft.com/wdsi/filesubmission/) для передачи файлов для анализа.</span><span class="sxs-lookup"><span data-stu-id="e6877-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="e6877-108">Знаете ли вы, что вы можете включить защиту безопасных ссылок для внутренних сообщений, отправляемых между получателями в вашей организации?</span><span class="sxs-lookup"><span data-stu-id="e6877-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="e6877-109">Выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e6877-109">Follow these steps:</span></span>

  1. <span data-ttu-id="e6877-110">Перейдите к [https://protection.office.com](https://protection.office.com) учетной записи глобального администратора или администратора безопасности и войдите в нее.</span><span class="sxs-lookup"><span data-stu-id="e6877-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="e6877-111">В левой области навигации в разделе **Управление угрозами** выберите **пункт** \> **безопасные ссылки** .</span><span class="sxs-lookup"><span data-stu-id="e6877-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="e6877-112">В разделе **политики, которые применяются ко всей Организации** , выберите политику и нажмите кнопку **изменить** .</span><span class="sxs-lookup"><span data-stu-id="e6877-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="e6877-113">В разделе **Параметры включите параметр** **применять безопасные ссылки к сообщениям, отправляемым в Организации** .</span><span class="sxs-lookup"><span data-stu-id="e6877-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>

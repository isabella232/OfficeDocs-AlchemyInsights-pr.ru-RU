---
title: Поиск и удаление сообщений электронной почты в вашей организации
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500968"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="782cc-102">Поиск и удаление сообщений электронной почты в вашей организации</span><span class="sxs-lookup"><span data-stu-id="782cc-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="782cc-103">Выполните приведенные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="782cc-103">Follow these steps:</span></span>

1. <span data-ttu-id="782cc-104">Если вы не глобальный администратор, для поиска сообщений ваша учетная запись должна быть добавлена в группу ролей **диспетчера** электронных поисков или роль управления поиском **соответствия** требованиям.</span><span class="sxs-lookup"><span data-stu-id="782cc-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="782cc-105">Чтобы удалить сообщения, необходимо присоединиться к группе ролей **управления** организацией или роли управления поиском и **очисткой.**</span><span class="sxs-lookup"><span data-stu-id="782cc-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="782cc-106">Разрешения на эти роли назначены в центре [& соответствия требованиям.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="782cc-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="782cc-107">[Создайте поиск контента,](https://docs.microsoft.com/office365/securitycompliance/content-search) чтобы найти удаление сообщения.</span><span class="sxs-lookup"><span data-stu-id="782cc-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="782cc-108">[Подключение к Центру безопасности и соответствия требованиям Windows PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="782cc-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="782cc-109">Если вы используете MFA, см. в этих инструкциях: Подключение к центру & безопасности PowerShell с помощью [многофакторной проверки подлинности](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="782cc-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="782cc-110">Удаление сообщения: запустите `New-ComplianceSearchAction` cmdlet, чтобы удалить сообщение.</span><span class="sxs-lookup"><span data-stu-id="782cc-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="782cc-111">Удаленные сообщения перемещаются в папку "Извлекаемые элементы" пользователя.</span><span class="sxs-lookup"><span data-stu-id="782cc-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="782cc-112">Пример команды см. в [шаге 3. Удаление сообщения.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="782cc-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>

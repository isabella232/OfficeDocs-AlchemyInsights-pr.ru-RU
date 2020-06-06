---
title: При исправлении приложений Microsoft 365, связанных с лицензиями Office, не удалось найти сообщение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580454"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="f7bb5-102">Исправление сообщения о том, что приложение Microsoft 365 "не удалось найти связанные с лицензиями Office"</span><span class="sxs-lookup"><span data-stu-id="f7bb5-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="f7bb5-103">Если вы получили это сообщение, попробуйте следующее:</span><span class="sxs-lookup"><span data-stu-id="f7bb5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f7bb5-104">Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют Интернет-доступ к приложениям Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f7bb5-105">См.: [URL-адреса и диапазоны IP-адресов Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f7bb5-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="f7bb5-106">Удалите и [переназначите лицензию на Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="f7bb5-107">Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="f7bb5-108">Откройте раздел Параметры Windows > **учетных**записей & учетных записей  >  **электронной почты**и удалите все рабочие учетные записи, кроме затронутой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="f7bb5-109">Перейдите к разделу Параметры Windows > **учетных записей**  >  **работа или учебные**учетные записи и отключите все рабочие учетные записи, кроме затронутой учетной записи</span><span class="sxs-lookup"><span data-stu-id="f7bb5-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="f7bb5-110">Сбросьте состояние активации Office.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-110">Reset the Office activation state.</span></span> <span data-ttu-id="f7bb5-111">[Инструкции.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="f7bb5-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="f7bb5-112">[Выполните вход](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) , используя затронутую учетную запись пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7bb5-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="f7bb5-113">Дополнительные решения по устранению неполадок приведены [в статье нелицензированные продукты и ошибки активации в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="f7bb5-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
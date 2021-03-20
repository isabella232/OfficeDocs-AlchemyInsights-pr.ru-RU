---
title: Импорт и экспорт из Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898050"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="18902-102">Импорт и экспорт из Yammer</span><span class="sxs-lookup"><span data-stu-id="18902-102">Import and export from Yammer</span></span>

<span data-ttu-id="18902-103">**Импорт**</span><span class="sxs-lookup"><span data-stu-id="18902-103">**Import**</span></span>

<span data-ttu-id="18902-104">Возможности импорта пользователей зависят от того, находится ли сеть Yammer в [основном режиме для Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) или нет.</span><span class="sxs-lookup"><span data-stu-id="18902-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="18902-105">**Неосновной режим.** Пользователей можно импортировать в группы с помощью функции [Добавить из адресной книги](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (не более 100 пользователей) в окне параметров группы или в сеть с помощью [массового обновления](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в Администраторе сети.</span><span class="sxs-lookup"><span data-stu-id="18902-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="18902-106">**Основной режим.** Операции членства в группах и членства в сети следует выполнять на [портале администрирования Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [портале Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) или с помощью других функций Azure AD.</span><span class="sxs-lookup"><span data-stu-id="18902-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="18902-107">Сети в основном режиме больше не имеют доступа к массовому обновлению и другим устаревшим функциям.</span><span class="sxs-lookup"><span data-stu-id="18902-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="18902-108">В Yammer никогда не было возможности импорта содержимого из Администратора сети, даже если в другой сети использовалась функция экспорта данных.</span><span class="sxs-lookup"><span data-stu-id="18902-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="18902-109">Возможна повторная публикация контента с помощью решений партнеров или API Yammer REST.</span><span class="sxs-lookup"><span data-stu-id="18902-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="18902-110">**Экспорт**</span><span class="sxs-lookup"><span data-stu-id="18902-110">**Export**</span></span>

<span data-ttu-id="18902-111">[Функция экспорта сетевых данных в Администраторе сети](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) позволяет экспортировать контент из сетей Yammer, включая сообщения и файлы.</span><span class="sxs-lookup"><span data-stu-id="18902-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="18902-112">Вложения могут быть очень большими, что потребует продолжительного времени на выполнение экспорта.</span><span class="sxs-lookup"><span data-stu-id="18902-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="18902-113">Рекомендуется экспортировать активные сети с помощью [API экспорта данных](https://developer.yammer.com/docs/data-export-api) блоками за день или за неделю.</span><span class="sxs-lookup"><span data-stu-id="18902-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="18902-114">Служба поддержки Майкрософт не предлагает пользовательских сценариев для этой цели.</span><span class="sxs-lookup"><span data-stu-id="18902-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="18902-115">Имеется отдельная функция [экспорта GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) для экспорта контента отдельному пользователю.</span><span class="sxs-lookup"><span data-stu-id="18902-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>
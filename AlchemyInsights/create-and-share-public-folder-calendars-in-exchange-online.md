---
title: Создание общих календарей в общедоступных папках в Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712646"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="26e37-102">Создание общих календарей в общедоступных папках в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="26e37-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="26e37-103">Вы можете создать календарь в общедоступной папке только из классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="26e37-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="26e37-104">Чтобы настроить календари общедоступных папок, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="26e37-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="26e37-105">Убедитесь, что общедоступные папки развернуты в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="26e37-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="26e37-106">Дополнительные сведения см. в статье [Создание почтового ящика общедоступных папок](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span><span class="sxs-lookup"><span data-stu-id="26e37-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="26e37-107">Убедитесь, что вам назначены необходимые разрешения доступа для создания общедоступной папки.</span><span class="sxs-lookup"><span data-stu-id="26e37-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="26e37-108">Дополнительные сведения см. в статье [Разрешения общедоступных папок для Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="26e37-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="26e37-109">Войдите в классический клиент Outlook и убедитесь в наличии доступа к развернутой общедоступной папке.</span><span class="sxs-lookup"><span data-stu-id="26e37-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="26e37-110">Если вам не удается получить доступ к общедоступным папкам с помощью классического клиента Outlook, см. статью [Пользователи Exchange Online не могут подключаться к общедоступным папкам с помощью Outlook или OWA](https://aka.ms/pfcte).</span><span class="sxs-lookup"><span data-stu-id="26e37-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="26e37-111">Создайте новый тип календаря в общедоступной папке.</span><span class="sxs-lookup"><span data-stu-id="26e37-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="26e37-112">По умолчанию общедоступная папка предоставляется всем остальным пользователям.</span><span class="sxs-lookup"><span data-stu-id="26e37-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="26e37-113">Владелец общедоступной папки может изменить разрешения из классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="26e37-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="26e37-114">Дополнительные сведения см. в статье [Разрешения общедоступных папок для Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span><span class="sxs-lookup"><span data-stu-id="26e37-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="26e37-115">**Примечание.** Календари общедоступных папок предназначены для использования в организации и не могут быть опубликованы в Интернете.</span><span class="sxs-lookup"><span data-stu-id="26e37-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="26e37-116">Используйте общий почтовый ящик, если вы хотите опубликовать календарь в Интернете.</span><span class="sxs-lookup"><span data-stu-id="26e37-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>
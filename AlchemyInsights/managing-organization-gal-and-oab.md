---
title: Управление глобальным списком адресов и автономной адресной книгой организации
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022676"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="9e0ec-102">Управление глобальным списком адресов (GAL) и автономной адресной книгой (OAB) организации</span><span class="sxs-lookup"><span data-stu-id="9e0ec-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="9e0ec-103">Глобальный список адресов (GAL) — это список объектов, поддерживающих почту (любой тип получателей, который может получать письма) в организации.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="9e0ec-104">В каждой организации автоматически создается один глобальный список адресов.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="9e0ec-105">Вы можете создавать дополнительные глобальные списки адресов, чтобы разделить пользователей по организациям или расположениям, но один пользователь может одновременно просматривать и использовать только один глобальный список адресов.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="9e0ec-106">Некоторые почтовые клиенты, такие как Outlook для Windows, скачивают глобальный список адресов (GAL) для автономного использования.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="9e0ec-107">Это называется автономной адресной книгой (OAB).</span><span class="sxs-lookup"><span data-stu-id="9e0ec-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="9e0ec-108">В Exchange Online автономная адресная книга обновляется каждые 8 часов, после чего клиенты должны скачать ее для обновления своей локальной копии OAB.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="9e0ec-109">Любые изменения получателей должны сначала отобразиться в GAL, чтобы затем внести их в OAB.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="9e0ec-110">Некоторые распространенные процедуры GAL и OAB:</span><span class="sxs-lookup"><span data-stu-id="9e0ec-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="9e0ec-111">По ряду причин вам может потребоваться скрыть некоторые объекты в глобальном списке адресов.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="9e0ec-112">Сведения см. в разделе [Скрытие получателей из списков адресов](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="9e0ec-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="9e0ec-113">Если вам нужно предоставить определенным группам пользователей настроенные представления глобального списка адресов организации, см. статью [Политики адресных книг в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="9e0ec-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="9e0ec-114">[Создайте глобальный список адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), а чтобы узнать, как использовать разрешения GAL, см. статью [Списки адресов в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="9e0ec-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="9e0ec-115">Обратите внимание, что при создании GAL вам также может потребоваться создать OAB.</span><span class="sxs-lookup"><span data-stu-id="9e0ec-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="9e0ec-116">См. статью [Процедуры автономной адресной книги](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="9e0ec-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>

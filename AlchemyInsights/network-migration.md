---
title: Миграция сети
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799577"
---
# <a name="network-migration"></a><span data-ttu-id="7e90b-102">Миграция сети</span><span class="sxs-lookup"><span data-stu-id="7e90b-102">Network Migration</span></span>

<span data-ttu-id="7e90b-103">Клиент O365 может быть связан с несколькими сетями Yammer в клиенте 1: Конфигурация "многие сети".</span><span class="sxs-lookup"><span data-stu-id="7e90b-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="7e90b-104">Начиная с 16 октября, 2018 в Yammer больше не будет поддерживаться несколько сетей Yammer, связанных с одним клиентом.</span><span class="sxs-lookup"><span data-stu-id="7e90b-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="7e90b-105">Можно выполнить миграцию по сети, чтобы перейти к предпочтительной конфигурации 1:1.</span><span class="sxs-lookup"><span data-stu-id="7e90b-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="7e90b-106">Чтобы просмотреть список сетей, связанных с клиентом, выполните вход в Yammer в качестве глобального администратора и перейдите к **администратору сети**, а затем выполните **миграцию сети**.</span><span class="sxs-lookup"><span data-stu-id="7e90b-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="7e90b-107">Нажмите кнопку **Далее**.</span><span class="sxs-lookup"><span data-stu-id="7e90b-107">Choose **Next**.</span></span>

- <span data-ttu-id="7e90b-108">Если вы видите несколько сетей, перечисленных на этапе 2 из 3, то у вас есть несколько сетей Yammer, связанных с клиентом O365.</span><span class="sxs-lookup"><span data-stu-id="7e90b-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="7e90b-109">Чтобы изменить конфигурацию до 1:1, продолжайте использовать средство миграции сети.</span><span class="sxs-lookup"><span data-stu-id="7e90b-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="7e90b-110">Дополнительные сведения о миграции сети можно найти в статье [Перенос сети: объединение нескольких сетей Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="7e90b-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="7e90b-111">Обратите внимание:</span><span class="sxs-lookup"><span data-stu-id="7e90b-111">Please Note:</span></span>
  
- <span data-ttu-id="7e90b-112">**Миграция сети переносит только активных и ожидающих пользователей.**</span><span class="sxs-lookup"><span data-stu-id="7e90b-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="7e90b-113">Вместе с активными пользователями сведения о пользователях, такие как имя и изображение профиля, также переносятся.</span><span class="sxs-lookup"><span data-stu-id="7e90b-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="7e90b-114">Все сетевые содержимое, включая группы, не переносятся.</span><span class="sxs-lookup"><span data-stu-id="7e90b-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="7e90b-115">**Миграция сети не может быть отменена.**</span><span class="sxs-lookup"><span data-stu-id="7e90b-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="7e90b-116">После миграции вы не сможете получить доступ к своей сети и ее контенту.</span><span class="sxs-lookup"><span data-stu-id="7e90b-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="7e90b-117">Поэтому прежде чем приступать к миграции, необходимо тщательно спланировать эту ситуацию.</span><span class="sxs-lookup"><span data-stu-id="7e90b-117">So before you consider a migration, you want to plan carefully.</span></span>

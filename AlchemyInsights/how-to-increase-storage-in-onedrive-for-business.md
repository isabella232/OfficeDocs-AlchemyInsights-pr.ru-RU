---
title: Как увеличить хранилище в OneDrive для бизнеса
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780108"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="26cd4-102">Как увеличить хранилище в OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="26cd4-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="26cd4-103">Чтобы изменить хранилище по умолчанию для новых и существующих пользователей OneDrive, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="26cd4-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="26cd4-104">Перейдите на [страницу "хранение" в центре администрирования OneDrive](https://admin.onedrive.com/?v=StorageSettings)и введите новое значение в ГБ.</span><span class="sxs-lookup"><span data-stu-id="26cd4-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="26cd4-105">Этот параметр дискового пространства применяется ко всем пользователям, для которых не были заданы определенные пределы хранилища.</span><span class="sxs-lookup"><span data-stu-id="26cd4-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="26cd4-106">Чтобы изменить дисковое пространство для определенных пользователей, необходимо использовать Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="26cd4-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="26cd4-107">Сведения о том, как это сделать, можно узнать в статье [изменение места для хранения пользователей в OneDrive с помощью PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span><span class="sxs-lookup"><span data-stu-id="26cd4-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="26cd4-108">**Обратите внимание**: у вас нет плана, включающего неограниченное хранилище.</span><span class="sxs-lookup"><span data-stu-id="26cd4-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="26cd4-109">Сведения о хранилище, которое поставляется с каждым планом, можно узнать в статье [Описание службы OneDrive для бизнеса](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span><span class="sxs-lookup"><span data-stu-id="26cd4-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="26cd4-110">Чтобы увеличить объем хранилища в OneDrive для бизнеса, выберите подписку, которая включает **onedrive для бизнеса (план 2** ) или **Office 365 корпоративный E3**.</span><span class="sxs-lookup"><span data-stu-id="26cd4-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="26cd4-111">Чтобы изменить планы, в центре администрирования Microsoft 365 перейдите на страницу **выставление счетов** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** и выберите подписку, которую нужно изменить, а затем перейдите на вкладку **Обновление** .</span><span class="sxs-lookup"><span data-stu-id="26cd4-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="26cd4-112">Дополнительные сведения о переключении планов и хранилища OneDrive для бизнеса можно найти в [статье переключение на другой план Microsoft 365 для бизнеса](https://go.microsoft.com/fwlink/?LinkId=2031117) и [Описание службы onedrive для бизнеса](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span><span class="sxs-lookup"><span data-stu-id="26cd4-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>
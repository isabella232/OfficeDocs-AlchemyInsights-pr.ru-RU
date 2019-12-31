---
title: Совместное управление
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910416"
---
# <a name="co-management"></a><span data-ttu-id="2284f-102">Совместное управление</span><span class="sxs-lookup"><span data-stu-id="2284f-102">Co-management</span></span>

<span data-ttu-id="2284f-103">**Необходимые условия для миграции с гибридного диспетчера конфигураций в Intune**</span><span class="sxs-lookup"><span data-stu-id="2284f-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="2284f-104">Ознакомьтесь с [этой статьей](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="2284f-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="2284f-105">[Добавьте лицензию Intune для пользователей](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="2284f-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="2284f-106">При настройке совместного управления используйте [браузер пограничного сервера](https://www.microsoft.com/windows/microsoft-edge) .</span><span class="sxs-lookup"><span data-stu-id="2284f-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="2284f-107">**Как установить клиент диспетчера конфигураций на устройствах, управляемых Intune**</span><span class="sxs-lookup"><span data-stu-id="2284f-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="2284f-108">В этой статье представлены [устройства с Windows в системе Intune, управляемые MDM](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="2284f-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="2284f-109">**Что делать, если я хочу изменить только службу MDM?**</span><span class="sxs-lookup"><span data-stu-id="2284f-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="2284f-110">Службу MDM можно изменить, не открывая обращение в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="2284f-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="2284f-111">Изучите следующую документацию, чтобы помочь вам в изменении своего центра MDM:</span><span class="sxs-lookup"><span data-stu-id="2284f-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="2284f-112">Изменение полномочий MDM с диспетчера конфигураций на Intune standalone</span><span class="sxs-lookup"><span data-stu-id="2284f-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="2284f-113">Изменение центра MDM из Intune в качестве автономного в диспетчере конфигурации</span><span class="sxs-lookup"><span data-stu-id="2284f-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)
---
title: Код ошибки 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527050"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="9061b-103">Ошибка при активации Office 2013 в службах удаленных рабочих столов</span><span class="sxs-lookup"><span data-stu-id="9061b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="9061b-104">Если вы получаете сообщение об ошибке при активации Office 2013 для развертываний служб удаленных рабочих столов, рассмотрите возможность включения ADAL, изменив реестр.</span><span class="sxs-lookup"><span data-stu-id="9061b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="9061b-105">**Раздел реестра**</span><span class="sxs-lookup"><span data-stu-id="9061b-105">**Registry key**</span></span>|<span data-ttu-id="9061b-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="9061b-106">**Type**</span></span>|<span data-ttu-id="9061b-107">**Значение**</span><span class="sxs-lookup"><span data-stu-id="9061b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9061b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="9061b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="9061b-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="9061b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="9061b-110">1,1</span><span class="sxs-lookup"><span data-stu-id="9061b-110">1</span></span>  <br/> |

<span data-ttu-id="9061b-111">Дополнительную информацию можно узнать [в статье Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="9061b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="9061b-112">ADAL включается по умолчанию в Office 365 профессиональный плюс и Office 2016.</span><span class="sxs-lookup"><span data-stu-id="9061b-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="9061b-113">Службы удаленных рабочих столов (RDS) ранее назывались службами терминалов.</span><span class="sxs-lookup"><span data-stu-id="9061b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  
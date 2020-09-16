---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: cc6f93ba8ae3a030f83da5eca2d28dcf38f0f8f7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800909"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="f62df-102">Защита IRM для файлов SharePoint</span><span class="sxs-lookup"><span data-stu-id="f62df-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="f62df-103">В SharePoint Online защита IRM применяется к файлам на уровне списка и библиотеки.</span><span class="sxs-lookup"><span data-stu-id="f62df-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="f62df-104">Прежде чем ваша организация сможет использовать защиту IRM, сначала необходимо настроить управление правами.</span><span class="sxs-lookup"><span data-stu-id="f62df-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="f62df-105">Служба управления правами на доступ к данным Azure использует службу управления правами Azure из Azure Information Protection для шифрования и назначения ограничений на использование.</span><span class="sxs-lookup"><span data-stu-id="f62df-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="f62df-106">Некоторые подписки Microsoft 365 включают в себя управление правами Azure, но не все.</span><span class="sxs-lookup"><span data-stu-id="f62df-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="f62df-107">Дополнительные сведения см. в статьях</span><span class="sxs-lookup"><span data-stu-id="f62df-107">To learn more, see:</span></span>

- <span data-ttu-id="f62df-108">[Сведения о том, как приложения и службы Office поддерживают управление правами Azure](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span><span class="sxs-lookup"><span data-stu-id="f62df-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="f62df-109">[Настройка управления правами на доступ к данным (IRM) в центре администрирования SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span><span class="sxs-lookup"><span data-stu-id="f62df-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="f62df-110">[IRM — Включение библиотек документов и списков SharePoint](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span><span class="sxs-lookup"><span data-stu-id="f62df-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/microsoft-365/compliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="f62df-111">[Управление правами на доступ к данным в Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span><span class="sxs-lookup"><span data-stu-id="f62df-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="f62df-112">[Управление правами на доступ к данным в Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="f62df-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/information-rights-management-in-exchange-online).</span></span>



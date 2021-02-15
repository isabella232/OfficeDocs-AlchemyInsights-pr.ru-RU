---
title: Групповая политика
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243920"
---
# <a name="group-policy"></a><span data-ttu-id="6beb3-102">Групповая политика</span><span class="sxs-lookup"><span data-stu-id="6beb3-102">Group policy</span></span>

<span data-ttu-id="6beb3-103">Параметры для объектов пользователей и компьютеров в доменных службах Azure Active Directory (Azure AD DS) часто управляются с помощью объектов групповой политики (GPO).</span><span class="sxs-lookup"><span data-stu-id="6beb3-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="6beb3-104">Службы Azure AD DS содержат встроенные GPO для контейнеров AADDC Users и AADDC Computers.</span><span class="sxs-lookup"><span data-stu-id="6beb3-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="6beb3-105">Вы можете изменить эти встроенные GPO, чтобы настроить групповую политику под потребности своей среды.</span><span class="sxs-lookup"><span data-stu-id="6beb3-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="6beb3-106">Участники группы администраторов Azure AD DC обладают правами администрирования групповых политик в домене Azure AD DS, а также могут создавать настраиваемые GPO и подразделения.</span><span class="sxs-lookup"><span data-stu-id="6beb3-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="6beb3-107">Дополнительные сведения о том, что такое групповая политика и как она работает, см. в статье [Обзор групповой политики](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="6beb3-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="6beb3-108">В гибридной среде групповые политики, настроенные в локальной среде AD DS, не синхронизируются с Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="6beb3-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="6beb3-109">Чтобы определить параметры конфигурации для пользователей или компьютеров в Azure AD DS, измените один из стандартных объектов групповой политики или создайте собственный.</span><span class="sxs-lookup"><span data-stu-id="6beb3-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="6beb3-110">В статье [Управление групповой политикой](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) описано, как установить средства управления групповыми политиками, как изменить встроенные объекты групповой политики и как создать собственные объекты групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6beb3-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>




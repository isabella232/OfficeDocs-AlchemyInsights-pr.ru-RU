---
title: 646 как настроить AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779524"
---
# <a name="configure-sync-features"></a><span data-ttu-id="998e9-102">Настройка функций синхронизации</span><span class="sxs-lookup"><span data-stu-id="998e9-102">Configure sync features</span></span>

<span data-ttu-id="998e9-103">Azure AD Connect включает несколько функций, которые включены по умолчанию или могут быть включены позже.</span><span class="sxs-lookup"><span data-stu-id="998e9-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="998e9-104">Для некоторых функций требуется дополнительная настройка в определенных средах.</span><span class="sxs-lookup"><span data-stu-id="998e9-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="998e9-105">Ограничивающие [фильтры](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) объекты синхронизируются с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="998e9-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="998e9-106">По умолчанию синхронизируются все пользователи, контакты, группы и учетные записи компьютеров с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="998e9-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="998e9-107">Вы можете включить или исключить объекты, основанные на доменах, подРазделениях и других атрибутах.</span><span class="sxs-lookup"><span data-stu-id="998e9-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="998e9-108">[Хэш пароля синкронизатион](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизирует хэш пароля из локального каталога Active Directory с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="998e9-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="998e9-109">Это позволяет управлять паролями в одном месте, но использовать один и тот же пароль в локальной и облачной средах как в локальной среде, так и в облачной среде.</span><span class="sxs-lookup"><span data-stu-id="998e9-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="998e9-110">Так как Active Directory является достоверным источником, вы можете использовать собственные политики паролей.</span><span class="sxs-lookup"><span data-stu-id="998e9-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="998e9-111">[Самостоятельный сброс паролей (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволяет пользователям сбрасывать собственные пароли в облаке, не применяя локальную политику паролей.</span><span class="sxs-lookup"><span data-stu-id="998e9-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="998e9-112">[Обратная запись устройства](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволяет записывать зарегистрированные устройства в Azure AD обратно в локальную службу Active Directory, чтобы их можно было использовать для условного доступа.</span><span class="sxs-lookup"><span data-stu-id="998e9-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="998e9-113">[Защита от случайных удалений](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) включена по умолчанию для предотвращения слишком большого числа одновременных удалений объектов (более 500 объектов в каждой синхронизации).</span><span class="sxs-lookup"><span data-stu-id="998e9-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="998e9-114">Этот параметр можно изменить в соответствии с потребностями Организации.</span><span class="sxs-lookup"><span data-stu-id="998e9-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="998e9-115">[Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) включено по умолчанию для Экспресс-установок и помогает убедиться в том, что ваша версия Azure AD Connect всегда актуальна.</span><span class="sxs-lookup"><span data-stu-id="998e9-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    


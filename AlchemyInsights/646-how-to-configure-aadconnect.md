---
title: 646 как настроить AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28308118"
---
# <a name="configure-sync-features"></a><span data-ttu-id="0c4af-102">Настройка функции синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0c4af-102">Configure sync features</span></span>

<span data-ttu-id="0c4af-p101">Подключение Azure AD включает в себя ряд функций, включены по умолчанию, или можно включить более поздней версии. Некоторые функции требуется дополнительная настройка в конкретных средах.</span><span class="sxs-lookup"><span data-stu-id="0c4af-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="0c4af-p102">Ограничения для [фильтрации](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) объектов синхронизируются с Azure AD. По умолчанию все пользователи, контакты, группы и Windows 10 компьютера учетные записи синхронизированы. Можно включить или исключить объекты на основе доменов, подразделений или другие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="0c4af-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="0c4af-p103">[Хэш-функции синхронизации паролей](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизирует хэш пароля из локального Active Directory для Azure AD. Это позволяет управление паролями в одном месте, но использовать тот же пароль, как в локальных и облачных средах. Поскольку Active Directory авторитетным источником, можно использовать политик паролей.</span><span class="sxs-lookup"><span data-stu-id="0c4af-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="0c4af-111">[Самостоятельный сброс пароля (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволяет пользователям сбрасывать собственные пароли в облаке при применении политики паролей для локальной по-прежнему.</span><span class="sxs-lookup"><span data-stu-id="0c4af-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="0c4af-112">[Обратной записи устройства](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволяет зарегистрированных устройства в Azure AD записи в локальной Active Directory, они могут использоваться для условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0c4af-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="0c4af-p104">[Запретить случайное удаление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) включен по умолчанию для предотвращения удаления слишком большого числа одновременных объектов (более 500 объектов в синхронизации). Можно изменить этот параметр в соответствии с требованиями вашей организации.</span><span class="sxs-lookup"><span data-stu-id="0c4af-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="0c4af-115">[Автоматическое обновление](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) включен по умолчанию для установок express и обеспечивает вашей версии Azure AD подключение всегда является текущим.</span><span class="sxs-lookup"><span data-stu-id="0c4af-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    


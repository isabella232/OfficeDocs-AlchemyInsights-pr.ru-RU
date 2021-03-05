---
title: Синхронизация пароля
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449143"
---
# <a name="password-synchronization"></a><span data-ttu-id="3ce87-102">Синхронизация пароля</span><span class="sxs-lookup"><span data-stu-id="3ce87-102">Password synchronization</span></span>

<span data-ttu-id="3ce87-103">**Синхронизация с hash password не работает вообще**</span><span class="sxs-lookup"><span data-stu-id="3ce87-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="3ce87-104">Некоторые распространенные проблемы, с которыми сталкиваются клиенты, когда синхронизация с hash password не работает:</span><span class="sxs-lookup"><span data-stu-id="3ce87-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="3ce87-105">Учетной записи Active Directory, используемой Azure AD Connect для связи  с локальной  службой Active Directory, не предоставляется изменение каталога репликации, а каталог репликации изменяет все разрешения, необходимые для синхронизации паролей. Это необходимо исправить, выдав эти разрешения учетной записи Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3ce87-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="3ce87-106">Синхронизация хаширования паролей отключена после того, как  администратор изменил метод user Sign-In с синхронизации паролей на другой вариант, например Federation **с AD FS** в мастере Подключения Azure AD Connect. Это можно исправить, повторно включив функцию синхронизации с **hash** паролей в мастере Подключения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ce87-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="3ce87-107">Проблема подключения с локальной службой Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3ce87-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="3ce87-108">Например, некоторые контроллеры домена недоступны Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) или необходимые порты заблокированы брандмауэром. Это необходимо исправить, обеспечив правильное подключение между сервером Azure AD Connect и локальной службой Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3ce87-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="3ce87-109">Сервер Azure AD Connect в настоящее время находится в режиме постановки, из-за чего серверу не удастся получить хэши паролей. Чтобы устранить проблему, следуйте шагам, описанным в разделе Синхронизация паролей с синхронизацией [Azure AD Connect. Пароли](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)не синхронизируются.</span><span class="sxs-lookup"><span data-stu-id="3ce87-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="3ce87-110">**Синхронизация с hash password не работает для некоторых пользователей**</span><span class="sxs-lookup"><span data-stu-id="3ce87-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="3ce87-111">Если вы заметили, что hash паролей не  синхронизируется для пользователя, используйте задачу устранения неполадок в Azure AD Connect для расследования и устранения проблемы.</span><span class="sxs-lookup"><span data-stu-id="3ce87-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="3ce87-112">Выполните следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="3ce87-112">Perform the following tasks:</span></span>

    <span data-ttu-id="3ce87-113">а)</span><span class="sxs-lookup"><span data-stu-id="3ce87-113">a.</span></span> [<span data-ttu-id="3ce87-114">Выполнить задачу устранения неполадок в мастере</span><span class="sxs-lookup"><span data-stu-id="3ce87-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="3ce87-115">б)</span><span class="sxs-lookup"><span data-stu-id="3ce87-115">b.</span></span> [<span data-ttu-id="3ce87-116">Используйте командалет устранения неполадок, чтобы исследовать проблему синхронизации хаши пароля для определенного использования</span><span class="sxs-lookup"><span data-stu-id="3ce87-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="3ce87-117">Локальное устройство Active Directory User включено для пользователя, который должен изменить пароль **при следующем параметре logon.**</span><span class="sxs-lookup"><span data-stu-id="3ce87-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="3ce87-118">Когда этот параметр включен, пользователю назначен временный пароль и ему будет предложено изменить пароль на следующем логотипе.</span><span class="sxs-lookup"><span data-stu-id="3ce87-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="3ce87-119">Azure AD Connect не синхронизирует временные пароли с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ce87-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="3ce87-120">Чтобы устранить вышеуказанную проблему, выполните любой из следующих задач:</span><span class="sxs-lookup"><span data-stu-id="3ce87-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="3ce87-121">Попросите пользователя войти в локальное приложение (например, Windows Desktop) и изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="3ce87-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="3ce87-122">Новый пароль будет синхронизирован с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ce87-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="3ce87-123">У администратора обновить пароль пользователя без включения параметра **Пользователь** должен изменить пароль на следующем логотипе, и поделиться новым паролем с пользователем.</span><span class="sxs-lookup"><span data-stu-id="3ce87-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="3ce87-124">Локально объект Active Directory User  неправильно настроен для синхронизации объектов или синхронизации паролей.</span><span class="sxs-lookup"><span data-stu-id="3ce87-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="3ce87-125">Чтобы устранить эту проблему, выполните действия, описанные в синхронизации с помощью синхронизации паролей [с помощью синхронизации Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="3ce87-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>








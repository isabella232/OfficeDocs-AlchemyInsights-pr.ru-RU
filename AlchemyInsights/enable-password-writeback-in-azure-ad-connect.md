---
title: Разрешение обратной записи пароля в Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093368"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="9afd9-102">Разрешение обратной записи пароля в Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9afd9-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="9afd9-103">Чтобы включить обратную запись сброса пароля самообслуживания, сначала включите функцию обратной записи в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9afd9-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="9afd9-104">На сервере Azure AD Connect выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="9afd9-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="9afd9-105">Войдите на сервер Azure AD Connect и запустите мастер настройки **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="9afd9-106">На **странице приветствия** нажмите кнопку **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="9afd9-107">На странице **Дополнительные задачи** выберите **Настройка параметров синхронизации** и нажмите кнопку **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="9afd9-108">На странице Подключение к Azure AD введите учетные данные глобального администратора для вашего клиента Azure и нажмите кнопку "Продолжить".</span><span class="sxs-lookup"><span data-stu-id="9afd9-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="9afd9-109">На страницах фильтрации **Подключение каталогов** и **Домен/OU** нажмите **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="9afd9-110">На странице **Дополнительные возможности** выберите поле рядом с пунктом **Обратная запись пароля** и нажмите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="9afd9-111">На странице **Готово к настройке** нажмите кнопку **Настроить** и дождитесь завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="9afd9-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="9afd9-112">После завершения настройки нажмите кнопку **Выход**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="9afd9-113">Теперь с помощью обратной записи пароля, разрешенной в Azure AD Connect, можно настроить Azure AD SSPR для обратной записи.</span><span class="sxs-lookup"><span data-stu-id="9afd9-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="9afd9-114">Чтобы включить обратную запись пароля в SSPR, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="9afd9-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="9afd9-115">Войдите на портал Azure, используя учетную запись глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="9afd9-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="9afd9-116">Найдите и выберите **Azure Active Directory**, щелкните **Сброс пароля**, а затем выберите **Локальная интеграция**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="9afd9-117">Установите для параметра **Выполнять обратную запись паролей в локальный каталог?** значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="9afd9-118">Задайте для параметра **Разрешить пользователям разблокирование учетных записей без сброса пароля?** значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="9afd9-119">По завершении нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="9afd9-119">When ready, click **Save**.</span></span>

<span data-ttu-id="9afd9-120">Дополнительные сведения см. в статье [Включение обратной записи сброса пароля самообслуживания в Azure Active Directory для локальной среды](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="9afd9-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="9afd9-121">Когда администратор сбрасывает пароль пользователя на портале Azure Portal, пароль обратно записывается в локальной среде, если этот пользователь является федеративным или выполнена синхронизация хэша паролей.</span><span class="sxs-lookup"><span data-stu-id="9afd9-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="9afd9-122">Эта функция требует наличия лицензии Azure Premium (P1 или P2) и в настоящее время не поддерживается на портале администрирования Office.</span><span class="sxs-lookup"><span data-stu-id="9afd9-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>

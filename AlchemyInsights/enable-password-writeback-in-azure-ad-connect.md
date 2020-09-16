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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709740"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="aa118-102">Разрешение обратной записи пароля в Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="aa118-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="aa118-103">Чтобы включить обратную запись сброса пароля самообслуживания, сначала включите функцию обратной записи в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="aa118-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="aa118-104">На сервере Azure AD Connect выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="aa118-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="aa118-105">Войдите на сервер Azure AD Connect и запустите мастер настройки **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="aa118-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="aa118-106">На **странице приветствия** нажмите кнопку **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="aa118-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="aa118-107">На странице **Дополнительные задачи** выберите **Настройка параметров синхронизации** и нажмите кнопку **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="aa118-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="aa118-108">На странице **Подключение к Azure AD** введите учетные данные глобального администратора для вашего клиента Azure и нажмите кнопку "Продолжить".</span><span class="sxs-lookup"><span data-stu-id="aa118-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="aa118-109">На страницах фильтрации **Подключение каталогов** и **Домен/OU** нажмите **Продолжить**.</span><span class="sxs-lookup"><span data-stu-id="aa118-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="aa118-110">На странице **Дополнительные возможности** выберите поле рядом с пунктом **Обратная запись пароля** и нажмите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="aa118-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="aa118-111">На странице **Готово к настройке** нажмите кнопку **Настроить** и дождитесь завершения процесса.</span><span class="sxs-lookup"><span data-stu-id="aa118-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="aa118-112">После завершения настройки нажмите кнопку **Выход**.</span><span class="sxs-lookup"><span data-stu-id="aa118-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="aa118-113">Теперь с помощью обратной записи пароля, разрешенной в Azure AD Connect, можно настроить Azure AD SSPR для обратной записи.</span><span class="sxs-lookup"><span data-stu-id="aa118-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="aa118-114">Чтобы включить обратную запись пароля в SSPR, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="aa118-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="aa118-115">Войдите на портал Azure, используя учетную запись глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="aa118-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="aa118-116">Найдите и выберите **Azure Active Directory**, щелкните **Сброс пароля**, а затем выберите **Локальная интеграция**.</span><span class="sxs-lookup"><span data-stu-id="aa118-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="aa118-117">Установите для параметра **Выполнять обратную запись паролей в локальный каталог?** значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="aa118-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="aa118-118">Задайте для параметра **Разрешить пользователям разблокирование учетных записей без сброса пароля?** значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="aa118-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="aa118-119">По завершении нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="aa118-119">When ready, click **Save**.</span></span>

<span data-ttu-id="aa118-120">Дополнительные сведения см. в статье [Включение обратной записи сброса пароля самообслуживания в Azure Active Directory для локальной среды](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="aa118-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

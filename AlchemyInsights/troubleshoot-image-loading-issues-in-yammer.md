---
title: Устранение проблем с загрузкой изображений в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690256"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="92f0d-102">Устранение проблем с загрузкой изображений в Yammer</span><span class="sxs-lookup"><span data-stu-id="92f0d-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="92f0d-103">Когда возникают проблемы с фотографиями и предварительным просмотром файлов в Yammer, для устранения проблемы нужно проверить, возникает ли она у всех пользователей и на мобильных устройствах, а также можно ли ее воспроизвести при передаче вложения.</span><span class="sxs-lookup"><span data-stu-id="92f0d-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="92f0d-104">**Проблемы с фотографиями профилей**</span><span class="sxs-lookup"><span data-stu-id="92f0d-104">**Profile photo issues**</span></span>  

<span data-ttu-id="92f0d-105">Если конечные пользователи входят в Yammer через Microsoft 365, им нужно изменить свой профиль, включая фотографию профиля.</span><span class="sxs-lookup"><span data-stu-id="92f0d-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="92f0d-106">Если пользователям запрещено обновлять профили, эти действия может выполнить администратор.</span><span class="sxs-lookup"><span data-stu-id="92f0d-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="92f0d-107">Дополнительные сведения см. в статье [Просмотр и обновления профиля в Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="92f0d-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="92f0d-108">Сведения о редактировании профилей, включая фотографии профилей, см. в статье [Изменение профиля и настроек в Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="92f0d-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="92f0d-109">Обновленные фотографии профилей синхронизируются не так, как атрибуты профиля.</span><span class="sxs-lookup"><span data-stu-id="92f0d-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="92f0d-110">Чтобы запустить синхронизацию фотографии своего профиля, пользователь должен войти в систему.</span><span class="sxs-lookup"><span data-stu-id="92f0d-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="92f0d-111">Дополнительные сведения см. в статье [Обновляются ли изображения профилей пользователей из Office 365 в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="92f0d-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="92f0d-112">Сведения о жизненном цикле пользователей Yammer см. в статье [Управление пользователями Yammer через Office 365 на протяжении всего жизненного цикла](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="92f0d-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="92f0d-113">Сведения о том, как выполняется синхронизация изображений профиля в Microsoft 365, см. в статье [Информация о синхронизации изображений профилей в Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="92f0d-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="92f0d-114">**Проблемы с предварительным просмотром документов и с эскизами изображений**</span><span class="sxs-lookup"><span data-stu-id="92f0d-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="92f0d-115">Если файлы или изображения опубликованы в Yammer, предварительный просмотр может быть недоступен по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="92f0d-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="92f0d-116">Файл поврежден, поэтому его нельзя обработать.</span><span class="sxs-lookup"><span data-stu-id="92f0d-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="92f0d-117">Файл не был недавно добавлен в SharePoint Online, или Yammer по каким-либо иным причинам содержит недопустимые метаданные.</span><span class="sxs-lookup"><span data-stu-id="92f0d-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="92f0d-118">URL-адреса, необходимые для загрузки изображений предварительного просмотра, блокируются.</span><span class="sxs-lookup"><span data-stu-id="92f0d-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="92f0d-119">Версия файла для предварительного просмотра была удалена пользователем перед публикацией.</span><span class="sxs-lookup"><span data-stu-id="92f0d-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="92f0d-120">Версия для предварительного просмотра не была создана из-за проблемы со службой.</span><span class="sxs-lookup"><span data-stu-id="92f0d-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="92f0d-121">**Примечание.** Предварительный просмотр для ссылок и передачи файлов может работать по-разному.</span><span class="sxs-lookup"><span data-stu-id="92f0d-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="92f0d-122">Ссылки на файлы в интернете и ссылки, требующие дополнительной проверки подлинности, могут отображаться неправильно.</span><span class="sxs-lookup"><span data-stu-id="92f0d-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="92f0d-123">Дополнительные сведения см. в статье [Вложение файла или изображения в сообщение Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="92f0d-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 
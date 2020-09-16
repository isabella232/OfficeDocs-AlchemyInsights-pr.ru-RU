---
title: Проблема при открытии и скачивании файлов в Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695662"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="0f3c5-102">Проблема при открытии и скачивании файлов в Yammer</span><span class="sxs-lookup"><span data-stu-id="0f3c5-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="0f3c5-103">Классическая версия Yammer поддерживает несколько вариантов передачи файлов в сообщения и группы.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="0f3c5-104">В зависимости от конфигурации сети файлы по умолчанию хранятся в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="0f3c5-105">Средство выбора файлов в новой версии Yammer пока что поддерживает не все варианты, доступные в классической версии Yammer.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="0f3c5-106">В последующих обновлениях будут добавлены дополнительные возможности.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-106">A future update will add additional features.</span></span> <span data-ttu-id="0f3c5-107">Дополнительные сведения см. в статье [Вложение файла или изображения в сообщение беседы Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="0f3c5-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="0f3c5-108">**Не удается открыть или скачать файл**</span><span class="sxs-lookup"><span data-stu-id="0f3c5-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="0f3c5-109">Файл можно передать в Yammer, но также связан с файлом в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="0f3c5-110">Чтобы устранить проблему, сначала необходимо определить расположение файла.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="0f3c5-111">У файла, переданного в Yammer, будет URL-адрес \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="0f3c5-112">Убедитесь в том, что необходимые URL-адреса и IP-адреса не заблокированы.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="0f3c5-113">Дополнительные сведения см. в записи блога [Использование жестко закодированных IP-адресов для Yammer не рекомендуется](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="0f3c5-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="0f3c5-114">Выясните, может ли пользователь с правами глобального администратора скачать файл.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="0f3c5-115">Если файл является частным, может потребоваться использовать режим личного контента.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="0f3c5-116">Дополнительные сведения см. в статье [Отслеживание личного контента в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="0f3c5-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="0f3c5-117">**Гости и файлы на уровне сети Yammer в SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="0f3c5-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="0f3c5-118">[Гости на уровне сети в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не используют Azure AD B2B и являются внутренними по отношению к службе Yammer, поэтому они не могут получить доступ к файлам Yammer, хранящимся в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="0f3c5-119">Создайте внешнего пользователя AAD B2B, который сможет получать доступ к библиотекам документов в SharePoint Online с помощью этого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0f3c5-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="0f3c5-120">Сведения о будущей поддержке гостей Azure AD B2B в Yammer см. в статье [Поддержка гостевых пользователей сегмента бизнес-бизнес (B2B) в предварительной версии Yammer: Условия для клиентов и часто задаваемые вопросы](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="0f3c5-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>
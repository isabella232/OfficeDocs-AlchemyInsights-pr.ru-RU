---
title: Изменение каналов обновления для приложений Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739840"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="f12c8-102">Изменение каналов обновления для приложений Office</span><span class="sxs-lookup"><span data-stu-id="f12c8-102">Change update channels for Office apps</span></span>

<span data-ttu-id="f12c8-103">Для новых экземпляров Office используйте параметры скачивания программного обеспечения Office, чтобы выбрать нужный канал обновления, а затем установите (или переустановите) приложения Office.</span><span class="sxs-lookup"><span data-stu-id="f12c8-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="f12c8-104">Подробнее см. в статье [Управление параметрами скачивания программного обеспечения в Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="f12c8-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="f12c8-105">**Примечание** Выбор канала обновления, сделанный с помощью параметров скачивания программного обеспечения Office, действителен для всех пользователей, выполняющих новую установку с помощью портала Office 365.</span><span class="sxs-lookup"><span data-stu-id="f12c8-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="f12c8-106">Подробнее см. [Скачивание, установка и переустановка Microsoft 365 или Office 2019 на ПК или Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="f12c8-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="f12c8-107">Чтобы перейти на другой канал обновления для существующих экземпляров Office, используйте средство развертывания Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="f12c8-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="f12c8-108">Скачайте последнюю версию средства ODT (setup.exe) в [Центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f12c8-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="f12c8-109">Укажите имя канала, на который вы хотите переключиться.</span><span class="sxs-lookup"><span data-stu-id="f12c8-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="f12c8-110">Дополнительные сведения см. в статье [Параметры конфигурации для средства развертывания Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="f12c8-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="f12c8-111">Создайте конфигурационный XML-файл, указав название соответствующего канала, например update.xml.</span><span class="sxs-lookup"><span data-stu-id="f12c8-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="f12c8-112">Из командной строки для администратора перейдите в папку, где расположен файл setup.exe, и введите следующую команду:</span><span class="sxs-lookup"><span data-stu-id="f12c8-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="f12c8-113">а.</span><span class="sxs-lookup"><span data-stu-id="f12c8-113">a.</span></span> <span data-ttu-id="f12c8-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="f12c8-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="f12c8-115">Запустите приложение Office (например, Excel), а затем щелкните **Файл** > **Учетная запись**.</span><span class="sxs-lookup"><span data-stu-id="f12c8-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="f12c8-116">В разделе "Сведения о продукте" выберите **Параметры обновления** > **Обновить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="f12c8-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="f12c8-117">Подробнее см. в статье [Как перейти на другой канал обновления для существующих приложений Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="f12c8-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="f12c8-118">Чтобы переключиться на канал обновления для выбранной группы пользователей или с помощью диспетчера конфигураций (SCCM), настройте параметр канала обновления с помощью GPO.</span><span class="sxs-lookup"><span data-stu-id="f12c8-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="f12c8-119">Дополнительные сведения см. в статье [Обзор каналов обновления для Приложений Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="f12c8-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="f12c8-120">Подробнее см. в статье [Как управлять каналами Office 365 профессиональный плюс для ИТ-специалистов](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) и [Как управлять обновлениями Приложений Microsoft 365 с помощью Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="f12c8-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>
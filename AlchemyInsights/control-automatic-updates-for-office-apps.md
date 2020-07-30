---
title: Управление автоматическими обновлениями приложений Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431621"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="8f0c5-102">Управление автоматическими обновлениями приложений Office</span><span class="sxs-lookup"><span data-stu-id="8f0c5-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="8f0c5-103">По умолчанию обновления для приложений Office загружаются автоматически и применяются в фоновом режиме, без какого-либо вмешательства со стороны пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="8f0c5-104">При этом администраторы могут управлять порядком применения обновлений с помощью параметров обновления Office.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="8f0c5-105">С помощью параметров обновления администраторы могут включать и отключать автоматическое обновление, отображать или скрывать кнопку **Обновить сейчас** в Office, устанавливать крайние сроки обновлений и выполнять другие действия.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="8f0c5-106">Подробные сведения см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="8f0c5-106">For detailed information, see:</span></span>

- [<span data-ttu-id="8f0c5-107">Настройка параметров обновления для Office</span><span class="sxs-lookup"><span data-stu-id="8f0c5-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="8f0c5-108">Автоматическое обновление для Office не включено</span><span class="sxs-lookup"><span data-stu-id="8f0c5-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="8f0c5-109">Определение способа обновления Office после установки</span><span class="sxs-lookup"><span data-stu-id="8f0c5-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="8f0c5-110">Чтобы проверить существующие параметры обновления, примененные к клиентскому компьютеру, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="8f0c5-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="8f0c5-111">Откройте редактор реестра: нажмите кнопку **Пуск** > **Выполнить** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="8f0c5-112">Перейдите в следующее расположение и проверьте параметры обновления Office:</span><span class="sxs-lookup"><span data-stu-id="8f0c5-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="8f0c5-113">а.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-113">a.</span></span> <span data-ttu-id="8f0c5-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="8f0c5-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="8f0c5-115">b.</span><span class="sxs-lookup"><span data-stu-id="8f0c5-115">b.</span></span> <span data-ttu-id="8f0c5-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="8f0c5-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="8f0c5-117">**Примечание**. Если задан раздел реестра OfficeMgmtCOM, в окне **Office** > **Учетная запись** > **Обновления Office** может отображаться сообщение "Обновлениями управляет системный администратор".</span><span class="sxs-lookup"><span data-stu-id="8f0c5-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="8f0c5-118">Дополнительные сведения см. в статье [Управление обновлениями для Приложений Microsoft 365 с помощью Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="8f0c5-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  
---
title: Установите значение ClientAccessServerEnabled для True
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
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510003"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="b3aab-102">Установите значение ClientAccessServerEnabled для True</span><span class="sxs-lookup"><span data-stu-id="b3aab-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="b3aab-103">Если вы не можете открыть зашифрованное сообщение электронной почты и вместо этого увидеть вложение **rpmsg,** выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="b3aab-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="b3aab-104">Подключитесь к Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b3aab-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="b3aab-105">Чтобы подключиться к Exchange Online PowerShell, необходимо войти с помощью учетной записи глобального администратора или администратора Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3aab-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="b3aab-106">а)</span><span class="sxs-lookup"><span data-stu-id="b3aab-106">a.</span></span> <span data-ttu-id="b3aab-107">Откройте Windows PowerShell, а затем запустите следующую команду: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="b3aab-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="b3aab-108">б)</span><span class="sxs-lookup"><span data-stu-id="b3aab-108">b.</span></span> <span data-ttu-id="b3aab-109">В **диалоговом окне Windows PowerShell запроса** учетных данных введите свою учетную запись или учетную запись школы и пароль c.</span><span class="sxs-lookup"><span data-stu-id="b3aab-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="b3aab-110">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b3aab-110">Click **OK**.</span></span> 

2. <span data-ttu-id="b3aab-111">Запустите следующую команду, чтобы создать новый сеанс:</span><span class="sxs-lookup"><span data-stu-id="b3aab-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="b3aab-112">а)</span><span class="sxs-lookup"><span data-stu-id="b3aab-112">a.</span></span> <span data-ttu-id="b3aab-113">Выполните следующую команду:</span><span class="sxs-lookup"><span data-stu-id="b3aab-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="b3aab-114">Запустите `Get-IRMConfiguration` команду.</span><span class="sxs-lookup"><span data-stu-id="b3aab-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="b3aab-115">Проверьте параметр **ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="b3aab-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="b3aab-116">а)</span><span class="sxs-lookup"><span data-stu-id="b3aab-116">a.</span></span> <span data-ttu-id="b3aab-117">Если **параметр ClientAccessServerEnabled** настроен на **False,** запустите следующий cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="b3aab-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="b3aab-118">Всегда закройте сеанс powershell следующей командой: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="b3aab-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="b3aab-119">Дополнительные сведения см. в [веб-сайте Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="b3aab-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>


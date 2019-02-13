---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941727"
---
<span data-ttu-id="77f83-p101">Проблемы при архивации элементов в архивный почтовый ящик. Убедитесь в том, что выполнены следующие действия:</span><span class="sxs-lookup"><span data-stu-id="77f83-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="77f83-p102">Убедитесь, что **архив почтового ящика** был включен. Если нет, выполните действия в [этой статье](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , чтобы включить в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="77f83-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="77f83-106">В центре администрирования Exchange выберите **Теги хранения** в разделе **Управление соответствием требованиям**, создайте **тега хранения** с действием **Переместить в архив** , содержащий желаемую **Срока хранения**.</span><span class="sxs-lookup"><span data-stu-id="77f83-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="77f83-107">В центре администрирования Exchange выберите **Политики хранения**, создайте **Политику хранения** и добавьте вашей **Переместить в архив** тега хранения для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77f83-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="77f83-p103">[Назначение политики хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для определенного пользователя почтового ящика. Та же политика будет применяться к **основной** и **архивного** почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="77f83-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="77f83-p104">Почтовый ящик пользователя должны появиться политики архивирования для перемещаются в архивный почтовый ящик. Может потребоваться принудительно управляемых папок Assistant (многофакторной проверкой Подлинности) для запуска и применения новых параметров почтового ящика пользователя. Выполните следующую команду при [подключенной к EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) запуск помощника для управляемых папок для определенного почтового ящика:</span><span class="sxs-lookup"><span data-stu-id="77f83-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="77f83-113">Дополнительные сведения о настройке политики архивирования, к разделу [Set архива и удаления политики почтовых ящиков](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="77f83-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  


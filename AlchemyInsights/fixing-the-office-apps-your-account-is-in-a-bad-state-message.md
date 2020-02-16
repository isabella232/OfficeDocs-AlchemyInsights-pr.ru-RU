---
title: Исправление приложений Office, в которых ваша учетная запись находится в ошибочном сообщении о состоянии
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969737"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="e038f-102">Исправление ошибки приложений Office "Ваша учетная запись находится в неправильном состоянии"</span><span class="sxs-lookup"><span data-stu-id="e038f-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="e038f-103">Чтобы устранить эту ошибку, попробуйте выполнить следующие действия на затронутом компьютере:</span><span class="sxs-lookup"><span data-stu-id="e038f-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="e038f-104">Откройте приложение Office, выберите пункт выйти из**учетной записи** >  **файла** > **выход из всех учетных записей**.</span><span class="sxs-lookup"><span data-stu-id="e038f-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="e038f-105">Повторно выполните вход, используя учетную запись пользователя с действительной лицензией.</span><span class="sxs-lookup"><span data-stu-id="e038f-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="e038f-106">Более подробную информацию можно узнать [в статье Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e038f-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e038f-107">[Очистите учетные данные Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощью диспетчера учетных данных Windows.</span><span class="sxs-lookup"><span data-stu-id="e038f-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="e038f-108">**Примечание:** Пути реестра для Office 2016 изменились на 16,0.</span><span class="sxs-lookup"><span data-stu-id="e038f-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e038f-109">Например, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="e038f-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="e038f-110">На затронутом компьютере установите параметр Енаблеадал = 0, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e038f-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="e038f-111">Щелкните правой кнопкой мыши кнопку Windows и выберите команду **выполнить**.</span><span class="sxs-lookup"><span data-stu-id="e038f-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="e038f-112">В поле **Открыть** введите **regedit**и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="e038f-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="e038f-113">Выберите **Да** , если будет предложено разрешить редактору реестра вносить изменения на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e038f-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e038f-114">В редакторе реестра добавьте значение DWORD Енаблеадал с параметром 0 в раздел HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="e038f-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="e038f-115">Если ошибка возникает при подключении к Office 365 с помощью Office 2013, [включите современная проверка подлинности](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) для клиента Office.</span><span class="sxs-lookup"><span data-stu-id="e038f-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="e038f-116">Дополнительные сведения см. [Устранение неполадок в приложениях, не являющихся браузерами, которые не могут войти в Office 365, Azure или Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="e038f-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>


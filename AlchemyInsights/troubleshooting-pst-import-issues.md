---
title: Устранение проблем с импортом PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991379"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="d1f1a-102">Устранение проблем с импортом PST</span><span class="sxs-lookup"><span data-stu-id="d1f1a-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="d1f1a-103">Если вы выполняете импорт в самом клиенте Outlook, см. [Устранение проблем с импортом .pst файла Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="d1f1a-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="d1f1a-104">Если вы используете службу импорта и она застряла, обратите внимание, что каждый PST-файл, который вы загружаете в расположение хранилища Azure, должен иметь размер не более 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="d1f1a-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="d1f1a-105">Файлы PST размером более 20 ГБ могут повлиять на производительность процесса импорта PST.</span><span class="sxs-lookup"><span data-stu-id="d1f1a-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="d1f1a-106">Если вы хотите проверить состояние определенного задания импорта, вы можете использовать [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="d1f1a-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="d1f1a-107">Для получения полной информации о сервисе импорта, см. [Обзор импорта файлов PST вашей организации](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d1f1a-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>

---
title: Устранение проблем с импортом PST
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
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757753"
---
# <a name="troubleshooting-pst-import-issues"></a>Устранение проблем с импортом PST

- Если вы выполняете импорт в самом клиенте Outlook, см. [Устранение проблем с импортом .pst файла Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Если вы используете службу импорта и она застряла, обратите внимание, что каждый PST-файл, который вы загружаете в расположение хранилища Azure, должен иметь размер не более 20 ГБ. Файлы PST размером более 20 ГБ могут повлиять на производительность процесса импорта PST.

- Если вы хотите проверить состояние определенного задания импорта, вы можете использовать [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Для получения полной информации о сервисе импорта, см. [Обзор импорта файлов PST вашей организации](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).

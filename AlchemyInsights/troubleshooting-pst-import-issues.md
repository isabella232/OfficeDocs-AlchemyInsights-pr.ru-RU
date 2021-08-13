---
title: Устранение проблем с импортом PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972432"
---
# <a name="troubleshooting-pst-import-issues"></a>Устранение проблем с импортом PST

- Если вы выполняете импорт в самом клиенте Outlook, см. статью [Устранение проблем с импортом PST-файла Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Если вы используете службу импорта и она зависла, обратите внимание, что каждый PST-файл, отправляемый в расположение службы хранилища Azure, не должен превышать 20 ГБ. Файлы PST размером более 20 ГБ могут повлиять на производительность процесса импорта PST-файлов. Дополнительные сведения об устранении неполадок с зависающими заданиями см. в статье [Проблемы, влияющие на задания импорта PST-файлов](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Если вы хотите проверить состояние определенного задания импорта, используйте [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Полные сведения о службе импорта см. в статье [Обзор импорта PST-файлов организации](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).

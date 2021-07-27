---
title: Ограничения меток конфиденциальности для файлов Office в SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: c3a0695dc2aa5f6e56be2235f08c81dbbe7fcea2
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533002"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Ограничения меток конфиденциальности для файлов Office в SharePoint и OneDrive

При включении меток конфиденциальности для файлов Office в SharePoint и OneDrive учитывайте требования и ограничения, в том числе:

- SharePoint и OneDrive не могут обрабатывать некоторые файлы, помеченные и зашифрованные в классических приложениях Office, если они содержат данные PowerQuery, данные, сохраняемые пользовательскими надстройками, или пользовательские XML-части.
- SharePoint и OneDrive не применяют метки конфиденциальности автоматически к существующим файлам, которые уже зашифрованы с помощью меток Azure Information Protection (AIP). Применение меток конфиденциальности к зашифрованным файлам: 
    - Перенесите метки AIP и опубликуйте их в Центре соответствия требованиям Microsoft 365.
    - Скачайте файлы с метками, а затем отправьте их в исходное расположение SharePoint или OneDrive.
- Для зашифрованных документов печать не поддерживается.

Дополнительные сведения об ограничениях см. в статье [Включение меток конфиденциальности для файлов Office в SharePoint и OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).

---
title: Соединять SharePoint библиотеку с сетевым диском
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: cd3d7d272552d5cd3f21f41160522001d79339d84a6d2259e1b1868deee66ef0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54087257"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Соединять SharePoint библиотеку с сетевым диском

Вместо сопоставления сетевого диска синхронизируйте SharePoint с новым клиентом приложение синхронизации OneDrive, который предоставляет файлы по запросу. Получите доступ ко всем своим файлам в OneDrive без использования локального хранилища. Дополнительные сведения см. в SharePoint и [Teams](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) файлы с компьютером и сохранить пространство диска с OneDrive Файлы по [запросу для Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

Если вы решите составить карту диска, а не использовать новый клиент [приложение синхронизации OneDrive,](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)убедитесь, что вы выполните следующие действия:

- [Устранение неполадок сопоставленных сетевых дисков, подключаемых к SharePoint Online](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Ошибки проверки подлинности возникают, когда у клиента нет поддержки TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**ПРИМЕЧАНИЕ:** Если вы используете Internet Explorer 10 с Windows 8 или Windows 7 и получаете  доступ отказано или путь не доступен при сопоставлении диска, уладите эту проблему, установив этот [hotfix](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d). 
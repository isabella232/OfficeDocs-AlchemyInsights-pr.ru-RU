---
title: Устранение неполадок производительности OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822211"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="4523f-102">Устранение неполадок производительности OneDrive</span><span class="sxs-lookup"><span data-stu-id="4523f-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="4523f-103">Если в OneDrive возникают медленные проблемы или аналогичные проблемы с производительностью, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="4523f-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="4523f-104">Убедитесь, что в [панели мониторинга работоспособности службы](https://portal.office.com/adminportal/home?ref=/servicehealth)нет известных проблем.</span><span class="sxs-lookup"><span data-stu-id="4523f-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="4523f-105">[Разрешите файлы по требованию](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) , чтобы получить доступ ко всем файлам в OneDrive без необходимости загружать их и использовать место на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4523f-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="4523f-106">[Ознакомьтесь](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) с рекомендациями по планированию и производительности сети.</span><span class="sxs-lookup"><span data-stu-id="4523f-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="4523f-107">[Максимизировать скорость передачи и загрузки](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), особенно если синхронизация устройства выполняется впервые.</span><span class="sxs-lookup"><span data-stu-id="4523f-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="4523f-108">Если вы синхронизируете библиотеку с более чем 100 000 элементами, синхронизация OneDrive может зависнуть в течение длительного времени, или отображается состояние обработки 0KB КСМБ ".</span><span class="sxs-lookup"><span data-stu-id="4523f-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="4523f-109">[Узнайте больше о синхронизации более 100 000 файлов](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , а также о [поддерживаемом в OneDrive ограничении файлов 300 000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="4523f-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="4523f-p102">Когда пользователь превышает ограничения на использование, SharePoint Online регулировки все последующие запросы из этой учетной записи пользователя в течение короткого периода. Все действия пользователя подвергаются регулированию время повтора.</span><span class="sxs-lookup"><span data-stu-id="4523f-p102">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period. All user actions are throttled while the throttle is in effect.</span></span>

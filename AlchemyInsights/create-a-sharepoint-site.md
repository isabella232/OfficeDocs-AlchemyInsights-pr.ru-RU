---
title: Создание сайта SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806952"
---
# <a name="create-a-sharepoint-site"></a>Создание сайта SharePoint

Создание сайтов и управление ими из [активных сайтов](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) в центре администрирования SharePoint. Дополнительные сведения см в разделе [Управление сайтами в новом центре администрирования SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Использованию

- **Невозможно** создать сайт с таким же URL-адресом существующего сайта. Если вы удалили сайт и хотите повторно использовать URL-адрес, то удаленный сайт по-прежнему будет существовать в разделе [удаленные сайты](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). Чтобы повторно использовать URL-адрес, необходимо окончательно удалить сайт. Чтобы полностью удалить сайт с помощью PowerShell, просмотрите пример командлета [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .
- Некоторые пользователи могут не иметь возможность создавать сайт. [В разделе Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Возможно, сайт зависает при **создании** дольше, чем ожидалось. Если вы пропустили эту ошибку более 24 часов, запишите запрос в службу поддержки. Во многих случаях мы уже работаем над решением. Отправьте нам по крайней мере 24 часа для завершения решения.

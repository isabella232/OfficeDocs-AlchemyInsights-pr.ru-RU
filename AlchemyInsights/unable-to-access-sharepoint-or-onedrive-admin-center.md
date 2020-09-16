---
title: Не удается получить доступ к Центру администрирования SharePoint или OneDrive
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
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749491"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Не удается получить доступ к Центру администрирования SharePoint или OneDrive

- Если сайт Центра администрирования SharePoint или OneDrive недоступен, возможно, возникла временная проблема со службой, из-за которой пользователи сталкиваются с периодическими задержками или ошибками перехода при обращении к сайтам SharePoint или контенту OneDrive. Проверьте [панель мониторинга работоспособности служб](https://admin.microsoft.com/AdminPortal/Home#/servicehealth), чтобы узнать, затронута ли ваша организация.

- Глобальным администраторам и администраторам SharePoint необходимо назначить лицензию SharePoint. Вновь созданные учетные записи, только что назначенные с лицензией SharePoint или ролью администратора, могут испытывать проблемы с доступом к SharePoint, такие как «доступ запрещен» или «пользователь не найден». Пожалуйста, дайте не менее 24 часов для синхронизации для всех наших систем. Мы понимаем, что 24 часа могут показаться долгим временем. Во многих случаях мы уже работаем над решением.

- Пользователям службы Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) может быть отказано в доступе, если окно времени доступа очень мало. См. статью [Отказ в доступе для учетных записей PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).
---
title: Проблемы с производительностью- SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093785"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive, недоступно или недоступно для нескольких пользователей

Если веб OneDrive или SharePoint не доступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная проблема с обслуживанием. [Проверьте панель мониторинга состояния службы.](https://portal.office.com/adminportal/home#/servicehealth)

**Добавление и лицензирование пользователя**

Убедитесь, что вы назначаете лицензии пользователям [в Microsoft 365 для бизнеса.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Назначение разрешений**

Если пользователю назначена лицензия Sharepoint и он по-прежнему получает сообщение об [](https://docs.microsoft.com/sharepoint/understanding-permission-levels) отказе в доступе, убедитесь, что ему назначен соответствующий уровень разрешений.

**Рассмотрите возможность использования функции запроса доступа**

Функция [запроса доступа](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, который в настоящее время не имеет разрешения на просмотр.

**Разрешение настраиваемой скрипт может привести к отказу в доступе**

Существуют определенные сценарии, в которых функция *Разрешить* настраиваемый сценарий может представлять отказ в доступе. Список затронутых функций, соображений безопасности и возможности отключить эту функцию. Пожалуйста, [посетите Разрешить или предотвратить настраиваемый сценарий](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


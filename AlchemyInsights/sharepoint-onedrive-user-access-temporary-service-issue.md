---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750569"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive работает медленнее, недоступно или недоступно для нескольких пользователей

Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы. [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).

**Добавление и лицензия пользователя**

Убедитесь, что вы [назначаете пользователям лицензии в Office 365 для бизнеса](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Назначение разрешений**

Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него назначен [соответствующий уровень разрешений](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Рассмотрите возможность использования функции запросов на доступ**

[Функция запросов на доступ](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения.

**Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом**

Существуют некоторые сценарии, в которых функции " *Разрешить пользовательскому сценарию* " может быть предоставлен отказ в доступе. Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции. Воспользуйтесь [разделом разрешить или запретить пользовательский сценарий](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


---
title: Проблемы с производительностью — SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719529"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint или OneDrive работает медленнее, недоступно или недоступно для нескольких пользователей

Если сайт OneDrive или SharePoint недоступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная ошибка службы. [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Добавление и лицензия пользователя

Убедитесь, что вы [назначаете пользователям лицензии в Office 365 для бизнеса](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Назначение разрешений

Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него назначен [соответствующий уровень разрешений](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) .

## <a name="consider-using-the-access-request-feature"></a>Рассмотрите возможность использования функции запросов на доступ

[Функция запросов на доступ](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом

Существуют некоторые сценарии, в которых функции " *Разрешить пользовательскому сценарию* " может быть предоставлен отказ в доступе. Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции. Воспользуйтесь разделом [Разрешить или запретить пользовательский сценарий](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


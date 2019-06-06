---
title: Устранение неполадок при доступе к сообщениям
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735750"
---
# <a name="troubleshoot-access-denied-messages"></a>Устранение неполадок при доступе к сообщениям

Если вы получаете сообщение об отказе в доступе при попытке просмотреть сайт SharePoint Online, ознакомьтесь со статьями ниже.

## <a name="add-and-license-the-user"></a>Добавление и лицензия пользователя

Убедитесь, что вы [назначаете пользователям лицензии в Office 365 для бизнеса](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).

Назначение разрешений

Если пользователю назначена лицензия SharePoint и по-прежнему получается сообщение об отказе в доступе, убедитесь, что для него [назначен соответствующий уровень разрешений](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).

Рассмотрите возможность использования функции запросов на доступ

Функция [запросов на доступ](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволяет пользователям запрашивать доступ к контенту, на просмотр которого у них нет разрешения. 

Разрешить настраиваемый скрипт может вызывать проблемы, связанные с доступом

Существует несколько сценариев, в которых функция "разрешить пользовательский сценарий" может привести к отказу в доступе. Список затронутых компонентов, рекомендации по безопасности и возможность отключения этой функции. Посетите, разрешите [или запретите использование настраиваемого скрипта](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script) .

Примечание. Если сайт OneDrive или SharePoint недоступен для нескольких пользователей, у которых ранее был доступ, может возникнуть временная ошибка службы. [Проверьте панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home#/servicehealth).


  


---
title: Устранение неполадок в доступе, отказано в сообщениях
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957986"
---
# <a name="troubleshoot-access-denied-messages"></a>Устранение неполадок в доступе, отказано в сообщениях

Если при попытке просмотреть веб-сайт Sharepoint Online вы получаете сообщение об отказе в доступе, см. ниже статьи.

**Добавление и лицензирование пользователя**

Убедитесь, что вы назначаете лицензии пользователям [в Microsoft 365 для бизнеса.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)

**Назначение разрешений**

Если пользователю назначена лицензия Sharepoint и он по-прежнему получает сообщение об отказе в доступе, убедитесь, что ему назначен соответствующий [уровень разрешений.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Рассмотрите возможность использования функции запроса доступа**

Функция [запроса](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) доступа позволяет пользователям запрашивать доступ к контенту, который в настоящее время не имеет разрешения на просмотр. 

**Разрешение настраиваемой скрипт может привести к отказу в доступе**

Существуют определенные сценарии, в которых функция "Разрешить настраиваемый сценарий" может представлять отказ в доступе. Список затронутых функций, соображений безопасности и возможности отключить эту функцию. Пожалуйста, посетите , [Разрешить или предотвратить настраиваемый сценарий](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Примечание. Если OneDrive или SharePoint не доступен нескольким пользователям, у которых ранее был доступ, может возникнуть временная проблема с обслуживанием. [Проверьте панель мониторинга состояния службы.](https://portal.office.com/adminportal/home#/servicehealth)


  


---
title: Отказано в доступе при сопоставлении диска с SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737490"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Устранение проблем с библиотеками SharePoint, сопоставленными с сетевыми дисками

При просмотре подключенного сетевого диска может появиться одно из следующих сообщений:
  
- **\\Путь недоступен. Возможно, у вас нет разрешения на использование этого сетевого ресурса. Обратитесь к администратору этого сервера, чтобы узнать, есть ли у вас разрешения на доступ.**

- **Доступ запрещен. Перед открытием файлов в этом расположении необходимо сначала добавить веб-сайт в список надежных сайтов, перейти на веб-сайт и выбрать автоматический вход.**

[Справка по устранению неполадок подключенных сетевых дисков](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
Сопоставление библиотеки как сетевого диска является временным и поддерживается только в Internet Explorer. Вместо этого [синхронизируйте файлы SharePoint с новым клиентом синхронизации OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , который включает [файлы по требованию](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Доступ ко всем файлам в OneDrive, не используя локальное дисковое пространство.
  
---
title: Отказано в доступе при сопоставлении диска с SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668756"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Устранение проблем с библиотеками SharePoint, сопоставленными с сетевыми дисками

При просмотре подключенного сетевого диска может появиться одно из следующих сообщений:
  
- **\\Путь недоступен. Возможно, у вас нет разрешения на использование этого сетевого ресурса. Обратитесь к администратору этого сервера, чтобы узнать, есть ли у вас разрешения на доступ.**

- **Доступ запрещен. Перед открытием файлов в этом расположении необходимо сначала добавить веб-сайт в список надежных сайтов, перейти на веб-сайт и выбрать автоматический вход.**

[Справка по устранению неполадок подключенных сетевых дисков](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
Сопоставление библиотеки как сетевого диска является временным и поддерживается только в Internet Explorer. Вместо этого [синхронизируйте файлы SharePoint с новым клиентом синхронизации OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , который включает [файлы по требованию](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Получите доступ ко всем своим файлам в OneDrive без использования локального хранилища.
  
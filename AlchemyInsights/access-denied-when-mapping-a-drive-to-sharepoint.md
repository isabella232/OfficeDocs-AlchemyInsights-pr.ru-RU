---
title: Доступ отказано при сопоставлении диска с SharePoint
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
ms.openlocfilehash: 1ed67ec926c3e73f7a16b927729255505dfe93a0ae442a5dff9400afafb41d8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938744"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Устранение проблем с SharePoint библиотек, относя к сетевым дискам

При просмотре на сетевом диске с картой можно увидеть одно из следующих сообщений:
  
- **\\Путь не доступен. Возможно, у вас нет разрешения на использование этого сетевого ресурса. Обратитесь к администратору этого сервера, чтобы узнать, есть ли у вас разрешения на доступ.**

- **Доступ отказано. Прежде чем открывать файлы в этом расположении, сначала необходимо добавить веб-сайт в список доверенных сайтов, просмотреть веб-сайт и выбрать вариант автоматического входа.**

[Получить справку по устранению неполадок, отбирающих сетевые диски.](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)
  
Сопоставление библиотеки как сетевого диска является временным и поддерживается только в Internet Explorer. Вместо этого [синхронизируйте SharePoint с новым клиентом приложение синхронизации OneDrive,](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) который включает файлы по [требованию.](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx) Получите доступ ко всем своим файлам в OneDrive без использования локального хранилища.
  
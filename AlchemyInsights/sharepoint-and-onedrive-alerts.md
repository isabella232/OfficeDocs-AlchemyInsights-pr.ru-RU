---
title: Задержки при получении оповещений SharePoint и OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742014"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Задержки при получении оповещений SharePoint и OneDrive

- Сначала проверьте папку нежелательной почты или спама.
- Если **задерживается все оповещения из нескольких файлов или библиотек**, перейдите на [панель мониторинга работоспособности службы](https://portal.office.com/adminportal/home?ref=/servicehealth) , чтобы проверить наличие помощников и инцидентов, которые могут возникнуть при работе с SharePoint или Exchange. Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange. Кроме того, обратите внимание на то, что отправляются другие сообщения электронной почты (если нет), то, скорее всего, есть задержки Exchange.
- Если **отдельное оповещение из определенного файла или библиотеки не доставлено**, попытайтесь удалить его и создать повторно. Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Оповещения не могут быть отправлены в группу рассылки. Поддерживаются только группы безопасности и O365.
> - Вы не можете настраивать шаблоны оповещений электронной почты. Для этого необходимо использовать Microsoft Flow или рабочий процесс SharePoint Designer.

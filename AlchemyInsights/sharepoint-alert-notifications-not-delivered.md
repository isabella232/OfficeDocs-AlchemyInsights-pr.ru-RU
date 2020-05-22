---
title: Уведомления о предупреждениях SharePoint не доставляются
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343090"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Уведомления о предупреждениях SharePoint не доставляются

Проверьте папку "Нежелательная почта" в электронной почте, как это может случиться в оповещениях.

Определите **, не доставлены ли все оповещения** или не доставлено **отдельное оповещение** из определенного файла или библиотеки.

- **Индивидуальные оповещения не доставляются**: Если отдельное оповещение из определенного файла или библиотеки не доставлено, вы можете попытаться удалить его и создать повторно. Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .
- **Все оповещения не доставляются**: Если все оповещения из нескольких файлов или библиотек не доставляются, перейдите на [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить наличие рекомендаций или инцидентов, которые могут возникнуть при работе с SharePoint или Exchange. Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange. Также обратите внимание на то, что отправляются другие сообщения электронной почты, а если нет, то эта ошибка, скорее всего, связана с задержками Exchange.

Вопросы и ответы по оповещениям:

- Невозможно отправлять оповещения в группу рассылки, поддерживаются только группы безопасности и группы Office 365.
- Вы не можете настраивать шаблоны оповещений по электронной почте; для достижения этих целей необходимо использовать Microsoft FLOW или рабочий процесс SharePoint Designer.

## <a name="related-topics"></a>Статьи по теме

Хотите попробовать Microsoft Flow в SharePoint Online?

- [Создание последовательности](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint и Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)

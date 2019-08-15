---
title: Уведомления о предупреждениях SharePoint не доставляются
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404815"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Уведомления о предупреждениях SharePoint не доставляются

Проверьте папку "Нежелательная почта" в электронной почте, как это может случиться в оповещениях.

Определите **, не доставлены ли все оповещения** или не доставлено **отдельное оповещение** из определенного файла или библиотеки.

- **Индивидуальные оповещения не**доставляются: Если отдельное оповещение из определенного файла или библиотеки не доставлено, вы можете попытаться удалить его и создать повторно. Для повторного создания оповещения в разделе [Управление, просмотр или удаление оповещений SharePoint](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) .
- **Все оповещения не**доставляются: Если все оповещения из нескольких файлов или библиотек не доставляются, перейдите на [панель мониторинга работоспособности службы](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , чтобы проверить наличие рекомендаций или инцидентов, которые могут возникнуть при работе с SharePoint или Exchange. Эта ошибка может быть связана с возможностью оповещений SharePoint или задержками в сообщениях электронной почты с помощью Exchange. Также обратите внимание на то, что отправляются другие сообщения электронной почты, а если нет, то эта ошибка, скорее всего, связана с задержками Exchange.

Вопросы и ответы по оповещениям:

- Невозможно отправлять оповещения в группу рассылки, поддерживаются только группы безопасности и группы Office 365.
- Вы не можете настраивать шаблоны оповещений по электронной почте; для достижения этих целей необходимо использовать Microsoft FLOW или рабочий процесс SharePoint Designer.

Дополнительные сведения:

- **Настройка оповещений**: Дополнительные сведения о настройке оповещений приведены [в статье Создание оповещения для получения уведомлений при изменении файлов и папок в SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Устранение неполадок оповещений**: Дополнительные сведения об устранении неполадок см. [Пользователи не получают уведомления о SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).
- Дополнительные сведения о политиках оповещений о **соответствии требованиям в O365**: Дополнительные сведения о настройке этих оповещений см. в разделе [политики оповещений о соответствии](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).
- **Журналы аудита SharePoint и OneDrive**: Дополнительные сведения о получении этих событий приведены [в статье Поиск в журнале аудита](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Оповещения, отправленные расширенной защитой от угроз**: Ознакомьтесь со статьей [ATP для SharePoint и OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Оповещения, отправляемые политиками защиты от потери данных**: просмотрите [уведомления по электронной почте для политик защиты от потери](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips)данных.

## <a name="related-topics"></a>Статьи по теме

Хотите попробовать Microsoft Flow в SharePoint Online?

- [Создание последовательности](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint и Flow](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)

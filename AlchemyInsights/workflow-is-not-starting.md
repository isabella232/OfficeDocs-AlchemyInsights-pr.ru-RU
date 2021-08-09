---
title: Рабочий процесс не начинается
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907751"
---
# <a name="workflow-is-not-starting"></a>Рабочий процесс не начинается

- SharePoint 2010 и SharePoint 2013 не начинаются.

    - Если рабочий процесс не начинается, может возникнуть временная проблема с обслуживанием, когда пользователи могут испытывать периодические задержки с прогрессом рабочего процесса. Проверьте панель [мониторинга состояния службы,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) чтобы узнать, влияет ли ваша организация на организацию.

    - Если прошло более 24 часов с тех пор, как вы впервые увидели эту проблему, зайдите в журнал билета поддержки. Во многих случаях мы уже работаем над решением. Пожалуйста, дайте нам по крайней мере 24 часа, чтобы завершить решение.

- SharePoint 2010 рабочий процесс отложен на запуск.

    - Это происходит, если рабочий процесс запускается большими партиями. (например, при добавлении сразу нескольких элементов).

    - Рабочий процесс не предназначен для запуска в режиме реального времени, поэтому задержка — это поведение по проекту.

   -  Если рабочий процесс является сложным языком разметки extensible object (XMOL), компиляция может быть медленной. Проверьте [эту](https://support.microsoft.com//kb/3043697) статью.

    - Необходимо упростить рабочий процесс или изменить его с помощью типа платформы microsoft SharePoint 2013.

    - Если ваша история рабочего процесса стала большой, может потребоваться очистить элементы или создать новый список истории.

        Дополнительные сведения: [История рабочего процесса очистки](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Похожие темы
Хотите попробовать Microsoft Flow в SharePoint Online?
- [Создание Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint и Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 

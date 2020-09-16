---
title: Веб-приложение OneDrive для бизнеса, перенаправляемое в delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776393"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Перенаправление на delve после нажатия кнопки OneDrive

Ознакомьтесь с подробным [руководством по устранению неполадок](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Чтобы устранить эту проблему, администратор должен предоставить пользователям право на создание сайта личных сайтов. Это связано с тем, что страница OneDrive для бизнеса создана на личных сайтах.

Чтобы предоставить это право, выполните указанные ниже действия.

1. В центре администрирования SharePoint выберите **Профили пользователей**.

2. В разделе **люди** выберите **Управление разрешениями пользователей**.

3. Добавьте пользователей, которым требуются разрешения на создание сайта личных сайтов. По умолчанию этому параметру присвоено значение **все, кроме внешних пользователей**.

4. После добавления пользователя, пользователей или группы убедитесь, что выбраны добавленные пользователи, пользователи или группы, перейдите к разделу **разрешения** , а затем установите флажок **создать личный сайт (требуется для личного хранилища, канала новостей и контента)**.

5. Нажмите кнопку **ОК**, а затем попросите пользователя открыть страницу OneDrive, чтобы создать сайт.

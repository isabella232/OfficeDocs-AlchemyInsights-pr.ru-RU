---
title: OneDrive для бизнеса Web OneDrive перенаправляет в Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800002"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Перенаправлено в Delve после нажатия OneDrive

См. в нашем [подробном руководстве по устранению неполадок.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Чтобы устранить эту проблему, администратор должен предоставить пользователям право создавать свой сайт "Мои сайты". Это происходит потому, что страница OneDrive для бизнеса создается на моих сайтах.

Чтобы предоставить это право, выполните следующие действия:

1. В центре администрирования SharePoint щелкните **профили пользователей.**

2. В разделе **Люди** нажмите **кнопку Управление разрешениями пользователей**.

3. Добавьте пользователей, которым требуются разрешения на создание сайта My Sites. По умолчанию этот параметр заданной для **всех, кроме внешних пользователей.**

4. После добавления пользователя, пользователей или группы убедитесь, что добавленный пользователь, пользователи или  группа выбраны, прокрутите в раздел разрешений, а затем выберите контрольный ящик рядом с Create Personal Site (необходимый для личного хранения, ленты новостей и **контента)**.

5. Нажмите **кнопку ОК,** а затем перейдите на страницу OneDrive, чтобы создать сайт.

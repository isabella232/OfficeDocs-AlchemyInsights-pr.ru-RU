---
title: OneDrive для бизнеса Веб-OneDrive перенаправляется в Delve
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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923000"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Перенаправлено Delve после нажатия OneDrive

См. в нашем [подробном руководстве по устранению неполадок.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Чтобы устранить эту проблему, администратор должен предоставить пользователям право создавать свой сайт "Мои сайты". Это происходит потому, что OneDrive для бизнеса страница создается на моих сайтах.

Чтобы предоставить это право, выполните следующие действия:

1. В центре администрирования SharePoint щелкните **профили пользователей.**

2. В разделе **Люди** нажмите **кнопку Управление разрешениями пользователей**.

3. Добавьте пользователей, которым требуются разрешения на создание сайта My Sites. По умолчанию этот параметр заданной для **всех, кроме внешних пользователей.**

4. После добавления пользователя, пользователей или группы убедитесь, что добавленный пользователь, пользователи или  группа выбраны, прокрутите в раздел разрешений, а затем выберите контрольный ящик рядом с Create Personal Site (необходимый для личного хранения, ленты новостей и **контента)**.

5. Нажмите **кнопку ОК,** а затем перейдите на страницу OneDrive, чтобы создать сайт.

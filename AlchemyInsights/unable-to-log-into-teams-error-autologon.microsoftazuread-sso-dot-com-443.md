---
title: Невозможно войти в Команды из-за ошибки autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038413"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Невозможно войти в Команды из-за ошибки autologon.microsoftazuread-sso dot com:443

Если в качестве аутентификации O365 включен бесшовный SSO, возможно, необходимо добавить URL-адрес autologon.microsoftazuread-sso.com в сайты интрасети.  Если он ранее был добавлен в доверенные сайты и используется бесшовная служба единого входа, его следует удалить из доверенных сайтов.

Пожалуйста, ознакомьтесь с [контрольным списком проблем с единой системой единого входа](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Выполните следующие действия, чтобы добавить URL-адрес в список сайтов интрасети:

1. Откройте Internet Explorer, нажав кнопку **Пуск**. В поле поиска введите Internet Explorer, а затем в списке результатов щелкните **Internet Explorer**.
2. Нажмите **Инструменты**, а затем нажмите **Свойства обозревателя**.
3. Щелкните вкладку **Безопасность**.
4. Теперь нажмите на **сайты локальной интрасети**, затем нажмите кнопку **сайтов** и затем кнопку **Дополнительно**.
5. Введите URL-адрес веб-сайта и нажмите **Добавить**.
6. Когда вы закончите, нажмите **Закрыть**.

Для получения дополнительной информации см. [Документация по развертыванию бесшовного единого входа для O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (включает процесс на основе политик для добавления URL-адреса на сайты интрасети на шаге 3).

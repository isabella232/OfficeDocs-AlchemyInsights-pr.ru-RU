---
title: Политика защиты приложений
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716906"
---
# <a name="application-protection-policy"></a>Политика защиты приложений

Если вы еще не работали с политикой защиты приложений (APP), см. статью [Обзор политик защиты приложений](https://docs.microsoft.com/intune/apps/app-protection-policy).

Прежде чем приступить к работе с политиками защиты приложений, см. статью [Как создавать и назначать политики защиты приложений](https://docs.microsoft.com/intune/app-protection-policies).

Требования к политике защиты приложений:

- У пользователя есть лицензия Intune или EMS.
- Пользователь входит в группу, для которой предназначены политики защиты приложений.
- Только один корпоративный пользователь выполнил вход в защищенные приложения на устройстве.
- Приложение реализовало пакет [SDK Intune](https://docs.microsoft.com/intune/app-sdk-get-started). Список приложений, поддерживающих пакет SDK, см. в статье [Приложения, защищенные Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Политики применяются после того, как пользователь, отвечающий приведенным выше требованиям, выполнит вход в приложение, поддерживающее пакет SDK Intune. Самый простой способ определить, применяется ли политика, — это потребовать, чтобы пользователь задал в политике ПИН-код. 

Дополнительные сведения см. в указанных ниже статьях.

[Вопросы и ответы по устранению неполадок APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Способ проверки настроек политики защиты приложений](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Общие сведения о времени доставки политики защиты приложений](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Как отслеживать политики защиты приложений](https://docs.microsoft.com/intune/app-protection-policies-monitor)
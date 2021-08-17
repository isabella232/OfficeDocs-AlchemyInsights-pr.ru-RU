---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e24f489292f38b5e9cacc8b9bfe5730ebfc71ce5e3004be479134ef6c791a12
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899345"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Оповещение сообщений электронной почты из "Фишинг доставлено из-за политики переопределения клиента или пользователя"

Политика оповещений по умолчанию с именем **Phish Delivered** из-за переопределения клиента или пользователя доступна в организациях с лицензиями Microsoft Defender для Office 365 P1 и P2. Если вы получили это оповещение, ниже следуют действия по расследованию:

1. Из сообщения оповещений щелкните **View Alert,** чтобы перейти на страницу Оповещений на Microsoft 365 Defender портале. 

2. Выберите оповещение, чтобы просмотреть **список** сообщений или **просмотреть сообщения в Explorer.** Оба этих параметра содержат сведения о сообщении, в котором содержится ID сообщения. Обратите внимание, что ссылка Обозреватель угроз автоматически фильтрует сообщения, которые соответствуют критериям оповещения. Возможно, потребуется настроить фильтр дат в Обозревателе угроз.

Сообщение фишинга было доставлено из-за переопределения вручную:

- Разрешенный отправитель или домен, установленный пользователем.
- Разрешенный отправитель или домен, установленный администратором в политике борьбы со спамом.
- Разрешенный IP-адрес в политике фильтра подключения.
- Правило потока почты (также известное как правило транспорта), настроенное для допуска сообщений.

Если вы считаете, что сообщение было неправильно помечено как фишинг, используйте [отправку администратора,](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) чтобы сообщить об этом сообщении в Корпорацию Майкрософт.

Пользователи могут использовать надстройку Report Message или надстройку [Report Phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) в Outlook для отправки образцов сообщений в Корпорацию Майкрософт.

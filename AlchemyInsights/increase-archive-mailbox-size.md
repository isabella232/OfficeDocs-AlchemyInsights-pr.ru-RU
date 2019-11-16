---
title: 305 увеличение размера архивного почтового ящика
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36661813"
---
# <a name="increase-the-archive-mailbox-size"></a>Увеличение размера архивного почтового ящика

Office 365 [ограничит](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) размер архивных почтовых ящиков на основе лицензии, назначенной учетной записи пользователя. Когда архивный почтовый ящик достигает 90% от разрешенного размера, пользователь получает уведомление по электронной почте. Если размер архивного почтового ящика достигает предела, пользователь не может переместить элементы в архивный почтовый ящик. Office 365 не приводит к увеличению размера архивного почтового ящика по достижении предельного размера. Вместо этого пользователи могут выполнить следующие действия, чтобы освободить место в архивном почтовом ящике:

- Экспортируйте элементы в PST-файл с помощью Outlook.

- Удаление элементов из архивного почтового ящика.

В Office 365 предоставляется **неограниченный Архив** для лицензий на Office 365 корпоративный E3 и водосостав. Администратор должен включить эту функцию до достижения максимального размера архивного почтового ящика. При включенном неограниченном архивировании в архивный почтовый ящик может уйти до 30 дней. Поэтому мы рекомендуем администраторам проверять свободное пространство в архивном почтовом ящике, что позволяет пользователю продолжать использовать архивный почтовый ящик при его развертывании. Дополнительные сведения [: обзор неограниченного архивирования в office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) и [Включение неограниченного архивирования в Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Дополнительные сведения о доступе к архивному почтовому ящику из Outlook можно узнать [в статье требования к Outlook для доступа к элементам в автоматически развернутом архиве](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Чтобы настроить политику хранения, которая автоматически перемещает элементы в архивный почтовый ящик, обратитесь к разделу [Настройка политики архивации и удаления для почтовых ящиков в организации Office 365](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Note**: автоматическое расширение архивов не поддерживается для основных почтовых ящиков в Exchange 2010.

---
title: Использование профилей электронной почты в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505214"
---
# <a name="using-email-profiles-with-intune"></a>Использование профилей электронной почты в Intune

Intune можно использовать для создания и развертывания профилей электронной почты для собственного (встроенного) почтового клиента на разных платформах устройств.

Сведения о некоторых ограничениях, связанных с профилями электронной почты, в том числе об обработке существующих профилей и их удалении, см. в статье [Добавление параметров электронной почты на устройства с помощью Intune](https://docs.microsoft.com/intune/email-settings-configure).

Дополнительные сведения о создании профилей электронной почты для каждой платформы см. в следующих статьях:

[Параметры устройств с Android для настройки электронной почты, проверки подлинности и синхронизации в Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Добавление параметров электронной почты на устройства iOS и iPadOS в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Параметры профиля электронной почты в Microsoft Intune для устройств с Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Параметры профиля электронной почты для устройств с Windows 10 в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Распространенная ошибка синхронизации**

**KNOX в профиле электронной почты для Android предотвращает синхронизацию контактов, календаря и задач пользователя с его устройствами.**

KNOX в профиле электронной почты для Android дает администратору возможность решить, какие типы контента синхронизировать с устройством. Для каждого из них необходимо установить значение "включено".

Если для какого-либо типа контента задано значение **Не настроен** (по умолчанию), этот тип контента не синхронизируется автоматически. Пользователь может включить нужный тип контента непосредственно на устройстве вручную, но такая конфигурация переопределяется параметром политики Intune, и синхронизация для этого типа контента прекращается.


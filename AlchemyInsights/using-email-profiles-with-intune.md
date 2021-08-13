---
title: Использование профилей электронной почты в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919436"
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


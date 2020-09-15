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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653301"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="e14a7-102">Использование профилей электронной почты в Intune</span><span class="sxs-lookup"><span data-stu-id="e14a7-102">Using email profiles with Intune</span></span>

<span data-ttu-id="e14a7-103">Intune можно использовать для создания и развертывания профилей электронной почты для собственного (встроенного) почтового клиента на разных платформах устройств.</span><span class="sxs-lookup"><span data-stu-id="e14a7-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="e14a7-104">Сведения о некоторых ограничениях, связанных с профилями электронной почты, в том числе об обработке существующих профилей и их удалении, см. в статье [Добавление параметров электронной почты на устройства с помощью Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="e14a7-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="e14a7-105">Дополнительные сведения о создании профилей электронной почты для каждой платформы см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="e14a7-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="e14a7-106">Параметры устройств с Android для настройки электронной почты, проверки подлинности и синхронизации в Intune</span><span class="sxs-lookup"><span data-stu-id="e14a7-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="e14a7-107">Добавление параметров электронной почты на устройства iOS и iPadOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e14a7-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="e14a7-108">Параметры профиля электронной почты в Microsoft Intune для устройств с Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="e14a7-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="e14a7-109">Параметры профиля электронной почты для устройств с Windows 10 в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e14a7-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="e14a7-110">**Распространенная ошибка синхронизации**</span><span class="sxs-lookup"><span data-stu-id="e14a7-110">**Common syncing issue**</span></span>

<span data-ttu-id="e14a7-111">**KNOX в профиле электронной почты для Android предотвращает синхронизацию контактов, календаря и задач пользователя с его устройствами.**</span><span class="sxs-lookup"><span data-stu-id="e14a7-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="e14a7-112">KNOX в профиле электронной почты для Android дает администратору возможность решить, какие типы контента синхронизировать с устройством. Для каждого из них необходимо установить значение "включено".</span><span class="sxs-lookup"><span data-stu-id="e14a7-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="e14a7-113">Если для какого-либо типа контента задано значение **Не настроен** (по умолчанию), этот тип контента не синхронизируется автоматически.</span><span class="sxs-lookup"><span data-stu-id="e14a7-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="e14a7-114">Пользователь может включить нужный тип контента непосредственно на устройстве вручную, но такая конфигурация переопределяется параметром политики Intune, и синхронизация для этого типа контента прекращается.</span><span class="sxs-lookup"><span data-stu-id="e14a7-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>


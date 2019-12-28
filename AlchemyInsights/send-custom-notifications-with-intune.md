---
title: Отправка настраиваемых уведомлений с помощью Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886870"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="fa3f4-102">Отправка настраиваемых уведомлений пользователям управляемых устройств с iOS и Android</span><span class="sxs-lookup"><span data-stu-id="fa3f4-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="fa3f4-103">Настраиваемые уведомления для Intune обрабатываются приложением "Корпоративный портал" на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="fa3f4-104">Затем приложение создает push-уведомление на этом устройстве.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="fa3f4-105">Ниже перечислены необходимые условия для поддержки получения настраиваемых уведомлений, а также для приложения, которое затем создает push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="fa3f4-106">На устройстве должно быть установлено приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="fa3f4-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="fa3f4-107">Устройство должно позволять приложению корпоративного портала отправлять push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="fa3f4-108">После установки или обновления приложения будет предложено разрешить пользователю отправлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="fa3f4-109">На устройствах с Android должны быть установлены службы Google проигрывания.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="fa3f4-110">Устройство должно быть зарегистрировано в Intune.</span><span class="sxs-lookup"><span data-stu-id="fa3f4-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="fa3f4-111">Дополнительные сведения о том, как отправить сообщение, можно найти в [документации по функциям](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="fa3f4-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>

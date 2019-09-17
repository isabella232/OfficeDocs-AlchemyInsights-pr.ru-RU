---
title: Отправка настраиваемых уведомлений с помощью Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992325"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="37e55-102">Отправка настраиваемых уведомлений пользователям управляемых устройств с iOS и Android</span><span class="sxs-lookup"><span data-stu-id="37e55-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="37e55-103">Настраиваемые уведомления для Intune обрабатываются приложением "Корпоративный портал" на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="37e55-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="37e55-104">Затем приложение создает push-уведомление на этом устройстве.</span><span class="sxs-lookup"><span data-stu-id="37e55-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="37e55-105">Ниже перечислены необходимые условия для поддержки получения настраиваемых уведомлений, а также для приложения, которое затем создает push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="37e55-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="37e55-106">На устройстве должно быть установлено приложение "Корпоративный портал".</span><span class="sxs-lookup"><span data-stu-id="37e55-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="37e55-107">Устройство должно позволять приложению корпоративного портала отправлять push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="37e55-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="37e55-108">После установки или обновления приложения будет предложено разрешить пользователю отправлять уведомления.</span><span class="sxs-lookup"><span data-stu-id="37e55-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="37e55-109">На устройствах с Android должны быть установлены службы Google проигрывания.</span><span class="sxs-lookup"><span data-stu-id="37e55-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="37e55-110">Устройство должно быть зарегистрировано в Intune.</span><span class="sxs-lookup"><span data-stu-id="37e55-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="37e55-111">Дополнительные сведения о том, как отправить сообщение, можно найти в [документации по функциям](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="37e55-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>

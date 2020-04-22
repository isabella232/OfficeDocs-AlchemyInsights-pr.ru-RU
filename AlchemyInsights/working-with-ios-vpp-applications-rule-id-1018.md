---
title: Работа с идентификатором правила приложений для iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719970"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="cd8eb-102">Работа с приложениями для iOS VPP</span><span class="sxs-lookup"><span data-stu-id="cd8eb-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="cd8eb-103">Узнайте, [как управлять приложениями для iOS, приобретенными через программу Volume-Purchase, с помощью Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , чтобы узнать о возможностях, ограничениях и действиях по использованию программы Apple Volume Purchase Program, а также ее поддержке в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cd8eb-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="cd8eb-104">**Распространенные проблемы:** "Мне назначено приложение для iOS VPP для пользователей, но не удалось выполнить установку".</span><span class="sxs-lookup"><span data-stu-id="cd8eb-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="cd8eb-105">Это может произойти, если один токен VPP используется для нескольких поставщиков услуг управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="cd8eb-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="cd8eb-106">Токены VPP от Apple можно использовать только с одним поставщиком.</span><span class="sxs-lookup"><span data-stu-id="cd8eb-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="cd8eb-107">Если вы использовали токен VPP с несколькими поставщиками, необходимо повторно отправить маркер в Intune.</span><span class="sxs-lookup"><span data-stu-id="cd8eb-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="cd8eb-108">Установка также может быть неисправной, если общее число установок превышает количество лицензий.</span><span class="sxs-lookup"><span data-stu-id="cd8eb-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="cd8eb-109">Чтобы просмотреть отчет об использовании лицензий, перейдите на страницу " \> **лицензии приложения** для **мобильных приложений Intune** ".</span><span class="sxs-lookup"><span data-stu-id="cd8eb-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="cd8eb-110">Сведения о том, как повторно использовать лицензии, можно найти в [этой статье.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="cd8eb-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>

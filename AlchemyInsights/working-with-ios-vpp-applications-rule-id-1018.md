---
title: Работа с iOS 1018 идентификатор правила VPP приложений
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29486585"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="4740a-102">Работа с iOS VPP приложений</span><span class="sxs-lookup"><span data-stu-id="4740a-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="4740a-103">Ознакомьтесь с [как управлять приложениями операций ввода-вывода, приобретенных через программу Корпоративная лицензия с Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) сведения о функциях, ограничения и шаги, чтобы использовать программы на покупку Apple тома и для него поддержку в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4740a-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="4740a-104">**Распространенные проблемы:** «Я назначается Мои пользователи приложения VPP операций ввода-вывода, но произошел сбой установки».</span><span class="sxs-lookup"><span data-stu-id="4740a-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="4740a-p101">Это может произойти при использовании одного маркера VPP между несколькими поставщиками управления мобильного устройства. Маркеры VPP из Apple может использоваться только с одного поставщика. При использовании маркера VPP с несколькими поставщиками, необходимо заново загрузите маркера, чтобы Intune.</span><span class="sxs-lookup"><span data-stu-id="4740a-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="4740a-p102">Установки также может не работать, если общее число установок количество лицензий. Чтобы просмотреть отчет об использовании для лицензий, перейдите к **Intune мобильного приложения** \> страницы **лицензий для приложений** . Чтобы узнать, как высвободить лицензии на использование, обратитесь к разделу [в этой статье.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="4740a-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    


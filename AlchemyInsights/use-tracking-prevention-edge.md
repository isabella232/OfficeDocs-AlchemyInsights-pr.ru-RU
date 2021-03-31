---
title: Использование блокировки отслеживания в Microsoft Edge (Chromium)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8328"
- "9004625"
ms.openlocfilehash: 09e9a7303063328cd7bd0a0fcbf9629a3b38ebb5
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51408789"
---
# <a name="use-tracking-prevention-in-microsoft-edge-chromium"></a><span data-ttu-id="334c2-102">Использование блокировки отслеживания в Microsoft Edge (Chromium)</span><span class="sxs-lookup"><span data-stu-id="334c2-102">Use tracking prevention in Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="334c2-103">Блокировка отслеживания в Microsoft Edge ограничивает доступ средства отслеживания к хранилищу браузера и сети.</span><span class="sxs-lookup"><span data-stu-id="334c2-103">Tracking prevention in Microsoft Edge limits a tracker's ability to access browser-based storage and the network.</span></span> <span data-ttu-id="334c2-104">Эта функция создана для соблюдения наших обязательств по обеспечению безопасности пользователей в Интернете с помощью Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="334c2-104">The feature is built to uphold our commitment to helping users stay safe on the web with Microsoft Edge.</span></span> <span data-ttu-id="334c2-105">Дополнительные сведения см. в статье [Блокировка отслеживания в Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) и разделе [Обязательство по конфиденциальности браузера](https://go.microsoft.com/fwlink/?linkid=2135350).</span><span class="sxs-lookup"><span data-stu-id="334c2-105">For more information, see [Tracking prevention in Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) and [Our browser privacy promise](https://go.microsoft.com/fwlink/?linkid=2135350).</span></span>

<span data-ttu-id="334c2-106">Microsoft Edge предлагает три уровня блокировки отслеживания (их можно выбрать на странице edge://settings/privacy):</span><span class="sxs-lookup"><span data-stu-id="334c2-106">Microsoft Edge offers three levels of tracking prevention (they can be selected in edge://settings/privacy):</span></span>

- <span data-ttu-id="334c2-107">**Базовая** является наименее строгой и предназначена для пользователей, которые наслаждаются персонализированными рекламными объявлениями и не против отслеживания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="334c2-107">**Basic** is the least restrictive and designed for users who enjoy personalized advertisements and don't mind being tracked on the web.</span></span> <span data-ttu-id="334c2-108">Базовая блокировка защищает пользователей только от вредоносных средств отслеживания, таких как сканеры отпечатков пальцев и майнеры криптовалюты.</span><span class="sxs-lookup"><span data-stu-id="334c2-108">Basic protects users only against malicious trackers, such as fingerprinters and cryptominers.</span></span>
- <span data-ttu-id="334c2-109">**Уравновешенная** является уровнем по умолчанию и предназначена для пользователей, которые хотят видеть меньше рекламных объявлений, следующих за ними в Интернете.</span><span class="sxs-lookup"><span data-stu-id="334c2-109">**Balanced** is the default level and designed for users who want to see fewer advertisements that follow them around the web.</span></span> <span data-ttu-id="334c2-110">Уравновешенный уровень направлен не только на блокировку средств отслеживания с сайтов, с которыми пользователи никогда не взаимодействовали, но и на минимизацию риска возникновения проблем совместимости.</span><span class="sxs-lookup"><span data-stu-id="334c2-110">Balanced level aims not only to block trackers from sites that users never engage with but also to minimize the risk of compatibility issues.</span></span>
- <span data-ttu-id="334c2-111">**Строгая** является наиболее строгой и предназначена для пользователей, которые готовы пожертвовать совместимостью веб-сайтов для обеспечения максимальной конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="334c2-111">**Strict** is the most restrictive and designed for users who don't mind sacrificing website compatibility for maximum privacy.</span></span>
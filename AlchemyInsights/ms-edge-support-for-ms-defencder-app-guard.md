---
title: Поддержка Microsoft Edge Application Guard для защитника Microsoft
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576634"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="c1313-102">Поддержка Microsoft Edge Application Guard для защитника Microsoft</span><span class="sxs-lookup"><span data-stu-id="c1313-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="c1313-103">Приложение Application Guard предназначено для Windows 10 и Microsoft EDGE, которое позволяет пользователю перемещаться по недоверенному сайту из изолированного контейнера с поддержкой Hyper-V, отделенного от операционной системы узла.</span><span class="sxs-lookup"><span data-stu-id="c1313-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="c1313-104">Администратор предприятия определяет список надежных веб-сайтов, облачных ресурсов и внутренних сетей.</span><span class="sxs-lookup"><span data-stu-id="c1313-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="c1313-105">Когда пользователь посещает сайт, которого нет в списке, Microsoft Edge откроет сайт в контейнере.</span><span class="sxs-lookup"><span data-stu-id="c1313-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="c1313-106">Это означает, что если сайт станет вредоносным, ведущий компьютер останется защищенным, а злоумышленник не получит доступ к корпоративным данным.</span><span class="sxs-lookup"><span data-stu-id="c1313-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="c1313-107">Установка расширений в контейнере поддерживается в Microsoft Edge версии 81, и ее можно контролировать с помощью политики.</span><span class="sxs-lookup"><span data-stu-id="c1313-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="c1313-108">Адрес Упдатеурл, который будет использоваться в политике Екстенсионинсталлфорцелист, должен быть добавлен в качестве нейтрального ресурса в политиках сетевой изоляции, используемых Application Guard.</span><span class="sxs-lookup"><span data-stu-id="c1313-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="c1313-109">Дополнительные сведения см. в разделе [Поддержка Microsoft Edge для Application Guard в защитнике Microsoft](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="c1313-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>

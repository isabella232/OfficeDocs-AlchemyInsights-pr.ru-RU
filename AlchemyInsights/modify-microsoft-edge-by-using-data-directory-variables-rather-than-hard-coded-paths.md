---
title: Изменение Microsoft Edge с помощью переменных каталога данных, а не жестко заданных путей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897895"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a><span data-ttu-id="cb45a-102">Изменение Microsoft Edge с помощью переменных каталога данных, а не жестко заданных путей</span><span class="sxs-lookup"><span data-stu-id="cb45a-102">Modify Microsoft Edge by using data directory variables rather than hard-coded paths</span></span>

<span data-ttu-id="cb45a-103">Например, чтобы в Windows сохранить данные профиля в локальных данных приложения пользователя, а не в расположении по умолчанию, установите для политики *UserDataDir* значение **${local_app_data}\Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="cb45a-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the *UserDataDir* policy to **${local_app_data}\Edge\Profile**.</span></span>

<span data-ttu-id="cb45a-104">Дополнительные сведения см. в статье [Создание переменных каталога пользовательских данных Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span><span class="sxs-lookup"><span data-stu-id="cb45a-104">For more information, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/microsoft-edge-policies).</span></span>
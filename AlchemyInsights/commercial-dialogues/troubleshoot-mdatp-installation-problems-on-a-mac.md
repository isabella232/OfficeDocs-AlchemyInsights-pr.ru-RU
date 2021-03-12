---
title: Устранение неполадок при установке MDATP на Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737661"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="e0a9d-102">Устранение неполадок при установке MDATP на Mac</span><span class="sxs-lookup"><span data-stu-id="e0a9d-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="e0a9d-103">Если не удается установить вручную, на странице **Сводка** мастера установки показано следующее:</span><span class="sxs-lookup"><span data-stu-id="e0a9d-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="e0a9d-104">"Ошибка произошла во время установки.</span><span class="sxs-lookup"><span data-stu-id="e0a9d-104">"An error occurred during installation.</span></span> <span data-ttu-id="e0a9d-105">Установщик столкнулся с ошибкой, из-за которой установка не справилась с работой.</span><span class="sxs-lookup"><span data-stu-id="e0a9d-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="e0a9d-106">Обратитесь за помощью к производителю программного обеспечения".</span><span class="sxs-lookup"><span data-stu-id="e0a9d-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="e0a9d-107">Для развертывания MDM на странице также показан общий сбой установки.</span><span class="sxs-lookup"><span data-stu-id="e0a9d-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="e0a9d-108">Хотя мы не отображаем точные ошибки конечным пользователям, мы храним файл журнала с ходом установки в **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="e0a9d-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="e0a9d-109">Каждый сеанс установки примыкает к этому файлу журнала.</span><span class="sxs-lookup"><span data-stu-id="e0a9d-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="e0a9d-110">Для вывода последнего сеанса установки используйте `sed` .</span><span class="sxs-lookup"><span data-stu-id="e0a9d-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="e0a9d-111">Дополнительные новости см. в выпуске Проблемы с установкой устранения неполадок [для MICROSOFT Defender ATP для Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="e0a9d-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>

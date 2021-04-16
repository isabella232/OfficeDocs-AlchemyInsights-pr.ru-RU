---
title: Дважды щелкнув файл Office, не удается открыть его
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814818"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="7bede-102">Дважды щелкнув файл Office, не удается открыть его</span><span class="sxs-lookup"><span data-stu-id="7bede-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="7bede-103">После двойного нажатия файла Office можно увидеть, что программа открыта, но сам файл не открывается.</span><span class="sxs-lookup"><span data-stu-id="7bede-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="7bede-104">Или вы можете получить ошибку: "Возникла проблема с отправкой команды в программу".</span><span class="sxs-lookup"><span data-stu-id="7bede-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="7bede-105">Причин для этого много, но наиболее распространенными решениями являются:</span><span class="sxs-lookup"><span data-stu-id="7bede-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="7bede-106">В Excel убедитесь, что параметр DDE не будет перепроверяться.</span><span class="sxs-lookup"><span data-stu-id="7bede-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="7bede-107">Этот параметр можно найти, создав новую книгу, а затем выбрав **файл > параметры > Advanced.**</span><span class="sxs-lookup"><span data-stu-id="7bede-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="7bede-108">В общем **разделе** отогнайте игнорировать другие приложения, которые используют Динамический обмен данными **(DDE).**</span><span class="sxs-lookup"><span data-stu-id="7bede-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="7bede-109">Запустите online Repair для восстановления параметров по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7bede-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="7bede-110">Щелкните кнопку "Начните с Windows" и выберите "Панель управления".</span><span class="sxs-lookup"><span data-stu-id="7bede-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="7bede-111">Откройте панель **управления** и перейдите к **программам > и функциям.**</span><span class="sxs-lookup"><span data-stu-id="7bede-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="7bede-112">Затем щелкните **правой кнопкой мыши Microsoft Office [Версия]** и выберите изменение > **Online Repair**.</span><span class="sxs-lookup"><span data-stu-id="7bede-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="7bede-113">Если ни одно из этих решений не работает, более полный список решений можно найти в статье поддержки, дважды щелкнув файл Office, не [откроет его.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="7bede-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>

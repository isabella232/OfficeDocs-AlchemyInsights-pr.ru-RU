---
title: Двойной щелчок файла Office не открывает его
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573596"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="e094e-102">Двойной щелчок файла Office не открывает его</span><span class="sxs-lookup"><span data-stu-id="e094e-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="e094e-103">После двойного щелчка файла Office можно увидеть, что программа открыта, но сам файл не открывается.</span><span class="sxs-lookup"><span data-stu-id="e094e-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="e094e-104">Или вы можете получить сообщение об ошибке: "ошибка при отправке команды программе".</span><span class="sxs-lookup"><span data-stu-id="e094e-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="e094e-105">Существует множество причин для этого, но двумя наиболее распространенными решениями являются:</span><span class="sxs-lookup"><span data-stu-id="e094e-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="e094e-106">В Excel убедитесь, что параметр DDE не установлен.</span><span class="sxs-lookup"><span data-stu-id="e094e-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="e094e-107">Этот параметр можно найти, создав новую книгу и выбрав **> параметры файлов > дополнительно**.</span><span class="sxs-lookup"><span data-stu-id="e094e-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="e094e-108">В разделе **Общие** снимите флажки **игнорировать другие приложения, использующие динамический обмен данными (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="e094e-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="e094e-109">Выполните оперативное восстановление для восстановления параметров по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e094e-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="e094e-110">Нажмите кнопку "Пуск" Windows и выполните поиск по запросу "Панель управления".</span><span class="sxs-lookup"><span data-stu-id="e094e-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="e094e-111">Откройте **Панель управления**и последовательно выберите пункты **программы > программы и компоненты**.</span><span class="sxs-lookup"><span data-stu-id="e094e-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="e094e-112">Затем щелкните правой кнопкой мыши **Microsoft Office [версия]** и выберите команду **изменить > оперативное восстановление**.</span><span class="sxs-lookup"><span data-stu-id="e094e-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="e094e-113">Если ни одно из этих решений не работает, в статье support можно найти более полный список решений, если [дважды щелкнуть файл Office, чтобы открыть его](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="e094e-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>

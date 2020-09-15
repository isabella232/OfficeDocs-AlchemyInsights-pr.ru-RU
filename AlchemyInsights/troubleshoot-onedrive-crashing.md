---
title: 'Устранение неполадок с OneDrive: аварийное завершение работы'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665011"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="11dfb-102">Устранение неполадок с OneDrive: аварийное завершение работы</span><span class="sxs-lookup"><span data-stu-id="11dfb-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="11dfb-103">Если OneDrive несколько раз аварийно завершает работу, сделайте следующее для устранения неполадок:</span><span class="sxs-lookup"><span data-stu-id="11dfb-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="11dfb-104">**Проверьте, что разделы реестра не заданы:**</span><span class="sxs-lookup"><span data-stu-id="11dfb-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="11dfb-105">Откройте редактор реестра и перейдите в раздел HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="11dfb-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="11dfb-106">Если параметр DisableFileSyncNGSC присутствует и его значение "1", откройте раздел и измените значение на "0".</span><span class="sxs-lookup"><span data-stu-id="11dfb-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="11dfb-107">Запуск OneDrive вручную через меню "Пуск"</span><span class="sxs-lookup"><span data-stu-id="11dfb-107">Manually launch OneDrive by going to Start</span></span> ![Нажмите клавишу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="11dfb-109">, введите "OneDrive" в поле поиска, а затем выберите классическое приложение OneDrive.</span><span class="sxs-lookup"><span data-stu-id="11dfb-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="11dfb-110">**Сброс OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="11dfb-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="11dfb-111">Примечания.</span><span class="sxs-lookup"><span data-stu-id="11dfb-111">Notes:</span></span>

- <span data-ttu-id="11dfb-112">Сброс OneDrive отключает все существующие подключения синхронизации (включая личный OneDrive, если была выполнена настройка).</span><span class="sxs-lookup"><span data-stu-id="11dfb-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="11dfb-113">Сброс OneDrive на компьютере не приведет к потере файлов и данных.</span><span class="sxs-lookup"><span data-stu-id="11dfb-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="11dfb-114">**Чтобы сбросить OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="11dfb-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="11dfb-115">Откройте диалоговое окно "Выполнить", нажав клавиши Windows+R.</span><span class="sxs-lookup"><span data-stu-id="11dfb-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="11dfb-116">Введите команду %localappdata%\Microsoft\OneDrive\onedrive.exe /reset и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="11dfb-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="11dfb-117">Ненадолго может появиться командное окно.</span><span class="sxs-lookup"><span data-stu-id="11dfb-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="11dfb-118">Запуск OneDrive вручную через меню "Пуск"</span><span class="sxs-lookup"><span data-stu-id="11dfb-118">Manually launch OneDrive by going to Start</span></span> ![Нажмите клавишу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="11dfb-120">, введите "OneDrive" в поле поиска, а затем выберите классическое приложение OneDrive.</span><span class="sxs-lookup"><span data-stu-id="11dfb-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="11dfb-121">Примечания.</span><span class="sxs-lookup"><span data-stu-id="11dfb-121">Notes:</span></span>

- <span data-ttu-id="11dfb-122">Если вы выбрали вариант синхронизации только некоторых папок перед сбросом, вам потребуется выполнить эти действия еще раз после завершения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="11dfb-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="11dfb-123">Дополнительные сведения см. в статье  [Выбор папок OneDrive для синхронизации с компьютером](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .</span><span class="sxs-lookup"><span data-stu-id="11dfb-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="11dfb-124">Вам потребуется проделать эти шаги для личного OneDrive и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="11dfb-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>
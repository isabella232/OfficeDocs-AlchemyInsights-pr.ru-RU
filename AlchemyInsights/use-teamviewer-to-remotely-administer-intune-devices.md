---
title: Удаленное администрирование устройств Intune с помощью TeamViewer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505213"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="98e5d-102">Удаленное администрирование устройств Intune с помощью TeamViewer</span><span class="sxs-lookup"><span data-stu-id="98e5d-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="98e5d-103">Устройства, управляемые Intune, можно администрировать удаленно с помощью [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="98e5d-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="98e5d-104">Чтобы администрировать Intune с помощью TeamViewer, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="98e5d-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="98e5d-105">Сначала получите учетные данные от TeamViewer, чтобы настроить соединитель TeamViewer в Intune.</span><span class="sxs-lookup"><span data-stu-id="98e5d-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="98e5d-106">Теперь администратор сможет ввести учетные данные в пользовательском интерфейсе соединителя TeamViewer в разделе "Устройства". Эта одноразовая операция нужна для установления связи между Intune и службой TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="98e5d-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="98e5d-107">**Часть 1. Начало сеанса с удаленным устройством**</span><span class="sxs-lookup"><span data-stu-id="98e5d-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="98e5d-108">В разделе **Все устройства** выберите устройство, с которым вы хотите начать сеанс удаленной работы.</span><span class="sxs-lookup"><span data-stu-id="98e5d-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="98e5d-109">Из меню **... Дополнительно** выберите пункт **Новый сеанс удаленного помощника**.</span><span class="sxs-lookup"><span data-stu-id="98e5d-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="98e5d-110">Нажмите **Да**, чтобы подтвердить, что хотите установить сеанс удаленной работы.</span><span class="sxs-lookup"><span data-stu-id="98e5d-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="98e5d-111">После того как служба TeamViewer подтвердит запрос "Запуск нового сеанса удаленной работы", вы увидите предложение **Начать сеанс удаленного помощника** под панелью "Обзор" (или "Основное") с подробными сведениями об устройстве.</span><span class="sxs-lookup"><span data-stu-id="98e5d-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="98e5d-112">Нажмите кнопку **Показать больше**, чтобы развернуть панель и отобразить состояние удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="98e5d-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="98e5d-113">Нажмите кнопку **Запустить удаленный сеанс**, чтобы запустить сеанс на стороне администратора.</span><span class="sxs-lookup"><span data-stu-id="98e5d-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="98e5d-114">Выберите скачивание бинарного файла TeamViewer (Windows) и нажмите **Выполнить**.</span><span class="sxs-lookup"><span data-stu-id="98e5d-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="98e5d-115">**Примечание.** Можно не обращать внимания на любые страницы веб-браузера, открытые на веб-сайте TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="98e5d-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="98e5d-116">Подтвердите запрос приложения TeamViewer на внесение изменений на устройстве (только Windows).</span><span class="sxs-lookup"><span data-stu-id="98e5d-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="98e5d-117">Приложение TeamViewer запустится и выведет код сеанса для проверки подлинности подключения к удаленному устройству.</span><span class="sxs-lookup"><span data-stu-id="98e5d-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="98e5d-118">**Часть 2. Действия на целевом устройстве сеанса удаленной работы**</span><span class="sxs-lookup"><span data-stu-id="98e5d-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="98e5d-119">Откройте портал компании Intune</span><span class="sxs-lookup"><span data-stu-id="98e5d-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="98e5d-120">Найдите флажок уведомления "Ваш администратор ИТ запрашивает доступ к управлению этим устройством для сеанса удаленного помощника" и нажмите на уведомление.</span><span class="sxs-lookup"><span data-stu-id="98e5d-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="98e5d-121">Выберите скачивание приложения TeamViewer или подтвердите скачивание приложения TeamViewer из App Store и нажмите **Выполнить**.</span><span class="sxs-lookup"><span data-stu-id="98e5d-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="98e5d-122">**Примечание.** Можно не обращать внимания на любые страницы веб-браузера, открытые на веб-сайте TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="98e5d-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="98e5d-123">Подтвердите запрос приложения TeamViewer на внесение изменений на устройстве (только Windows).</span><span class="sxs-lookup"><span data-stu-id="98e5d-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="98e5d-124">Приложение TeamViewer запустится и выведет код сеанса для проверки подлинности подключения к удаленному устройству.</span><span class="sxs-lookup"><span data-stu-id="98e5d-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="98e5d-125">Откроется всплывающее окно с запросом на разрешение запуска сеанса.</span><span class="sxs-lookup"><span data-stu-id="98e5d-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="98e5d-126">**Примечание.** Коды сеанса, созданные службой TeamViewer, являются одноразовыми.</span><span class="sxs-lookup"><span data-stu-id="98e5d-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="98e5d-127">При потере подключения необходимо выполнить следующие действия.</span><span class="sxs-lookup"><span data-stu-id="98e5d-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="98e5d-128">Закройте экземпляр приложения TeamViewer на удаленном устройстве и на рабочей станции администратора.</span><span class="sxs-lookup"><span data-stu-id="98e5d-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="98e5d-129">Закройте портал компании Intune на удаленном устройстве.</span><span class="sxs-lookup"><span data-stu-id="98e5d-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="98e5d-130">На портале администрирования создайте "Новый сеанс удаленного помощника".</span><span class="sxs-lookup"><span data-stu-id="98e5d-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="98e5d-131">Снова откройте портал компании Intune на удаленном устройстве, чтобы получить новое уведомление.</span><span class="sxs-lookup"><span data-stu-id="98e5d-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="98e5d-132">Повторно скачайте и откройте приложение TeamViewer и на удаленном устройстве, и на рабочей станции администратора.</span><span class="sxs-lookup"><span data-stu-id="98e5d-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>
---
title: Добавление подписи или отказ от глобальной компании для всех пользователей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465103"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="ab014-102">Добавление подписи или отказ от глобальной компании для всех пользователей</span><span class="sxs-lookup"><span data-stu-id="ab014-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="ab014-103">Совет. Подпись на всей организации также называется отказом от ответственности, независимо от того, что она включает.</span><span class="sxs-lookup"><span data-stu-id="ab014-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="ab014-104">В центре администрирования выберите **центры администрирования**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="ab014-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="ab014-105">В разделе "поток обработки почты" выберите пункт **правила**.</span><span class="sxs-lookup"><span data-stu-id="ab014-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="ab014-106">Щелкните значок " **+**" (Добавить) и выберите пункт **Применить заявления об отказе**.</span><span class="sxs-lookup"><span data-stu-id="ab014-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="ab014-107">Задайте имя правила.</span><span class="sxs-lookup"><span data-stu-id="ab014-107">Give the rule a name.</span></span>
5. <span data-ttu-id="ab014-108">В соответствии с этим правилом выберите **Apply для всех сообщений.**</span><span class="sxs-lookup"><span data-stu-id="ab014-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="ab014-109">В списке "Выполнить следующие действия..." оставьте выбранным пункт **Добавить в сообщение заявление об отказе**.</span><span class="sxs-lookup"><span data-stu-id="ab014-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="ab014-110">Щелкните ссылку **Введите текст** и введите заявление об отказе.</span><span class="sxs-lookup"><span data-stu-id="ab014-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="ab014-111">Нажмите **кнопку Выберите один,** **выберите Wrap** в качестве варианта отката, а затем нажмите **кнопку ОК**.</span><span class="sxs-lookup"><span data-stu-id="ab014-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="ab014-112">Это означает, что если заявление об отказе невозможно добавить из-за шифрования или других настроек почты, оно переносится в конверт сообщения.</span><span class="sxs-lookup"><span data-stu-id="ab014-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="ab014-113">Оставьте **аудит этого правила** с выбранным уровнем серьезности.</span><span class="sxs-lookup"><span data-stu-id="ab014-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="ab014-114">Затем выберите степень серьезности Низкая, Средняя или Высокая, которая будет использоваться в журнале сообщений.</span><span class="sxs-lookup"><span data-stu-id="ab014-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="ab014-115">Установите переключатель **Принудительно**, чтобы включить это правило немедленно, если его не нужно предварительно протестировать.</span><span class="sxs-lookup"><span data-stu-id="ab014-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="ab014-116">Щелкните ссылку **Дополнительные параметры**, чтобы добавить дополнительные условия или исключения.</span><span class="sxs-lookup"><span data-stu-id="ab014-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="ab014-117">По завершению нажмите **кнопку Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="ab014-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="ab014-118">Нужна дополнительная помощь?</span><span class="sxs-lookup"><span data-stu-id="ab014-118">Need more help?</span></span> [<span data-ttu-id="ab014-119">Просмотрите видео о создании отказов или ознакомьтесь с полной статьей.</span><span class="sxs-lookup"><span data-stu-id="ab014-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)
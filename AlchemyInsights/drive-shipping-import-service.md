---
title: Доставка дисков в службу импорта Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721724"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="10b4f-102">Доставка дисков в службу импорта Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="10b4f-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="10b4f-103">Используйте доставку диска, скопировав PST-файлы на жесткий диск, а затем отправив жесткий диск в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="10b4f-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="10b4f-104">Запуск задания:</span><span class="sxs-lookup"><span data-stu-id="10b4f-104">To start the job:</span></span>

1. <span data-ttu-id="10b4f-105">В Центре соответствия требованиям Microsoft 365 в разделе **Управление сведениями** выберите **Импорт**.</span><span class="sxs-lookup"><span data-stu-id="10b4f-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="10b4f-106">Выберите **Выбрать тип задания импорта**, а затем нажмите **Далее**.</span><span class="sxs-lookup"><span data-stu-id="10b4f-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="10b4f-107">Чтобы увидеть действия для этого варианта импорта, выберите **Доставка жестких дисков по адресу нашего фактического местонахождения**.</span><span class="sxs-lookup"><span data-stu-id="10b4f-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="10b4f-108">Помните:</span><span class="sxs-lookup"><span data-stu-id="10b4f-108">Here are some things to remember:</span></span>

- <span data-ttu-id="10b4f-109">Для импорта PST-файлов в почтовые ящики Microsoft 365 необходимо назначить роль экспорта-импорта почтовых ящиков в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="10b4f-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="10b4f-110">Производительность PTS-файлов размером более 20 ГБ может снизиться.</span><span class="sxs-lookup"><span data-stu-id="10b4f-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="10b4f-111">Можно использовать только 2,5-дюймовые твердотельные диски (SSD) и 2,5- или 3,5-дюймовые внутренние жесткие диски SATA II/III.</span><span class="sxs-lookup"><span data-stu-id="10b4f-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="10b4f-112">Жесткий диск, содержащий PST-файлы, должен быть зашифрован с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="10b4f-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="10b4f-113">Стоимость импорта PST-файлов в почтовые ящики Microsoft 365 при отправке жестких дисков в корпорацию Майкрософт составляет 2 доллара США за 1 ГБ данных.</span><span class="sxs-lookup"><span data-stu-id="10b4f-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="10b4f-114">Дополнительные сведения об использовании метода доставки дисков для импорта PST-файлов см. [Использование доставки дисков для импорта PST-файлов вашей организации](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="10b4f-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>
---
title: Открытие файла только для чтения
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 117b1e24d6250a1d5eb092a01a0d5146d09ea2e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903037"
---
# <a name="file-open-read-only"></a><span data-ttu-id="182c4-102">Открытие файла только для чтения</span><span class="sxs-lookup"><span data-stu-id="182c4-102">File open read-only</span></span>

<span data-ttu-id="182c4-p101">Может оказаться, что при открытии файлов, они открываются только для чтения. В некоторых случаях это для повышения безопасности, например, при открытии файлов из Интернета и в других случаях могут возникнуть из-за параметров, которые могут быть изменены. Ниже приведены некоторые действия, которые нужно выполнить для изменения и некоторые сценарии, когда файл открывает только для чтения.</span><span class="sxs-lookup"><span data-stu-id="182c4-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="182c4-106">**Мои антивирусная программа вызывает их открывать только для чтения**</span><span class="sxs-lookup"><span data-stu-id="182c4-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="182c4-p102">Некоторые антивирусной программы может защиты компьютера от потенциально небезопасных файлов, открывая их только для чтения. Может потребоваться обратитесь к поставщику антивирусного, чтобы узнать, как настроить эти параметры. BitDefender, например, содержит содержимое на добавление здесь исключения из приложения: [Добавление приложения или исключения для процессов в центре управления Bitdefender](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="182c4-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="182c4-110">**Свойства файла устанавливаются только для чтения?**</span><span class="sxs-lookup"><span data-stu-id="182c4-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="182c4-p103">Вы можете проверить свойства файла, щелкнув правой кнопкой мыши файл и выбрав пункт Свойства. Если установлен атрибут только для чтения, можно снимите соответствующий флажок и нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="182c4-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="182c4-113">**— Это содержимое в режиме защищенного просмотра**</span><span class="sxs-lookup"><span data-stu-id="182c4-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="182c4-p104">Файлы из Интернета и из других потенциально небезопасных расположений может содержать вирусов, червей или других вредоносных программ, которые могут вред. Это также часто в случае с вложений электронной почты или загрузки файлов. Чтобы защитить компьютер, файлы из этих потенциально небезопасных расположений открываются в режиме защищенного просмотра. С помощью режима защищенного просмотра можно чтение файла и просмотреть его содержимое снижает риски, связанные с. Дополнительные сведения о защищенный просмотр и изменение параметров см. в этой статье: [что такое защищенный?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="182c4-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="182c4-119">**Заполнен OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="182c4-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="182c4-p105">Если файл хранится на OneDrive и заполнен OneDrive место на диске, будет невозможно сохранить документ, пока не будете в разделе выделенное пространство. Свободное место на диске на OneDrive можно проверить, щелкнув значок OneDrive в центре уведомлений и выбрав Управление хранилища, или можно перейти к [http://onedrive.live.com](http://onedrive.live.com), вход и обратите внимание на то, исключаются дискового пространства, используемого в нижней части экрана.</span><span class="sxs-lookup"><span data-stu-id="182c4-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="182c4-122">**Office активации?**</span><span class="sxs-lookup"><span data-stu-id="182c4-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="182c4-p106">Если Office не активирован или истек срок действия подписки, может быть в режиме только для чтения ограниченной функциональности. Сведения о том, как для активации Office можно: [нелицензированный продукт и ошибок активации в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="182c4-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="182c4-125">**Найдя...**</span><span class="sxs-lookup"><span data-stu-id="182c4-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="182c4-126">Попробуйте перезагрузить компьютер</span><span class="sxs-lookup"><span data-stu-id="182c4-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="182c4-127">Установка обновлений Office</span><span class="sxs-lookup"><span data-stu-id="182c4-127">Install Office updates</span></span>
    
- <span data-ttu-id="182c4-128">Выполнять оперативное восстановление системы Office</span><span class="sxs-lookup"><span data-stu-id="182c4-128">Perform an Online repair of Office</span></span>
    


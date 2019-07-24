---
title: Проблемы с подключением SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840564"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблемы с подключением SharePoint Designer 

Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, воспользуйтесь следующими распространенными решениями.

Шаг 1: Убедитесь, что SharePoint Designer 2013 обновлен с помощью [SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) с пакетом обновления 1 и [обновлением 2 августа 2016 для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Шаг 2: очистите файлы локального кэша:

1. Закройте SharePoint Designer 2013.

2. На локальном компьютере удалите все файлы, найденные в каждой из следующих папок.

    - %Аппдата%\микрософт\веб Server Екстенсионс\каче
    - %Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче
    - %Усерпрофиле%\аппдата\локал\микрософт\вебситекаче

3. Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.

Шаг 3: [Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Шаг 4: администратору необходимо **Разрешить пользовательскому скрипту** в параметрах центра администрирования SharePoint разрешить подключение SharePoint Designer. Для [](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) получения дополнительных сведений см.



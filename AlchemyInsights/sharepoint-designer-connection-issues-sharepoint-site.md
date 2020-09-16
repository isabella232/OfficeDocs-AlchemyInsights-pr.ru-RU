---
title: Проблемы с подключением SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727184"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблемы с подключением SharePoint Designer 

Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, воспользуйтесь следующими распространенными решениями.

Шаг 1: Убедитесь, что SharePoint Designer 2013 обновлен с помощью [SharePoint Designer с пакетом обновления 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [обновлением 2 августа 2016 для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Шаг 2: очистите файлы локального кэша:

1. Закройте SharePoint Designer 2013.

2. На локальном компьютере удалите все файлы, найденные в каждой из следующих папок.

    - %Аппдата%\микрософт\веб Server Екстенсионс\каче
    - %Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче
    - %усерпрофиле%\аппдата\локал\микрософт\вебситекаче

3. Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.

Шаг 3: [Включение современной проверки подлинности для Office 2013 на устройствах с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Шаг 4: администратору необходимо **Разрешить пользовательскому скрипту** в параметрах центра администрирования SharePoint разрешить подключение SharePoint Designer. Для [получения](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) дополнительных сведений см.



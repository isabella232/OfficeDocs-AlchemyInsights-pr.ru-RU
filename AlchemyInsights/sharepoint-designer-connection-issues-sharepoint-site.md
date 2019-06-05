---
title: Уровни разрешений SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716904"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблемы с подключением SharePoint Designer 

<p>Если SharePoint Designer испытывает проблемы с подключением к сайтам SharePoint, попробуйте выполнить следующие распространенные решения.</p> <p><strong>Шаг 1:</strong> <strong>Проверка обновления&nbsp; SharePoint Designer</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">Пакет обновления 1 (SP1) для SharePoint Designer</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Обновление для SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Шаг 2:</strong> <strong>Очистка локальных файлов кэша</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Закройте SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">На локальном компьютере перейдите к следующим папкам, чтобы удалить кэшированные файлы.&nbsp;</li> <li style="font-weight: 400;">Нажмите кнопку <strong>Пуск&gt; — запустите</strong> и удалите все файлы, найденные в каждом из указанных ниже расположений.&nbsp;<br /><br />%Аппдата%\микрософт\веб Server Екстенсионс\каче<br />%Аппдата%\микрософт\шарепоинт Десигнер\проксяссембликаче<br />%Усерпрофиле%\аппдата\локал\микрософт\вебситекаче</li> <li style="font-weight: 400;">Откройте SharePoint Designer 2013 и снова введите учетную запись, чтобы проверить ее работу.</li> </ol> <p><strong>Шаг 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Включение современной проверки подлинности для Office 2013 на устройствах с Windows</strong></a>&nbsp;</p> <p><strong>Шаг 4:</strong> <strong>Администраторам необходимо разрешить пользовательскому сценарию разрешить подключение к SharePoint Designer</strong>.</p> <p>Подробное описание действий, примеры и рекомендации <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script"></a>см.&nbsp;</p>



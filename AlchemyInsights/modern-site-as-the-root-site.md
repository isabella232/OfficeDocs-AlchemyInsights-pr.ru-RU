---
title: Современный сайт в качестве корневого сайта
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057763"
---
# <a name="modern-site-as-root-site"></a>Современный сайт в качестве корневого сайта

Клиенты [целевого выпуска](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) теперь могут активировать интерфейс современного сайта для общения на классическом корневом сайте клиента SharePoint.

Эту функцию можно активировать, выполнив простой командлет PowerShell. При успешном выполнении команд PowerShell корневой сайт будет содержать новую домашнюю страницу сайта для общения. Сведения о командлетах и требованиях к функциям PowerShell доступны в статье [Enable – спокоммсите](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Мы будем постепенно отвлекаться по умолчанию, а не по умолчанию для клиентов, нацеленных на выпуск ранних версий 2019, а развертывание будет доступно в конце июня 2019. Продолжайте ссылаться на [Центр сообщений](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) о других новых возможностях с современным интерфейсом. 

**Важно!** не удаляйте классический корневой сайт для создания современного информационного сайта. Корпорация Майкрософт не поддерживает этот параметр. Удаление корневого сайта сделает все сайты SharePoint в Организации недоступными для всех пользователей, пока не восстановите сайт или не создаст новый сайт с тем же URL-АДРЕСом. 
 
 
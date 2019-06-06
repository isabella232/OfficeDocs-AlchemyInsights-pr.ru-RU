---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735155"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничение доступа в SharePoint или OneDrive

Существует множество способов ограничения доступа к службам SharePoint Online и OneDrive. Ниже приведено несколько способов ограничения доступа. 

Ограничение разрешений

В SharePoint Online и OneDrive для бизнеса мы ограничен доступ к элементам, таким как сайты, файлы и папки, только предоставляя доступ только тем группам и пользователям, у которых есть доступ.

[Настройка разрешений для списка или библиотеки SharePoint](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Настройка разрешений сайта в SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Изменение разрешений для вложенной папки](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Управление доступом с неуправляемых устройств](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

В SharePoint или глобальном администраторе в Office 365 вы можете заблокировать или ограничить доступ к контенту SharePoint и OneDrive с неуправляемых устройств (не с помощью гибридной среды AD или в Intune).

Ограничение расположения в сети

Администратор ИТ-администраторов может управлять доступом к ресурсам SharePoint и OneDrive на основе определенных сетевых расположений, которым вы доверяете. Это также называется политикой на основе расположения. Дополнительные сведения см. в статье [Управление доступом к данным SharePoint Online и OneDrive в зависимости от расположения в сети](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Ограничение блокировки сайта 

В SharePoint Online вы можете заблокировать семейство веб-сайтов, поэтому доступ к нему у него нет. Это задается с помощью PowerShell и [командной консоли SharePoint Online](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощью свойства [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

Запретить пользователям создавать сайты или дочерние сайты

Администратор SharePoint или глобальный администратор Office 365 позволяют пользователям создавать собственные сайты SharePoint и администрировать их, определять, какие сайты могут создаваться, и указывать расположение сайтов. Дополнительные сведения см. в статье [Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)


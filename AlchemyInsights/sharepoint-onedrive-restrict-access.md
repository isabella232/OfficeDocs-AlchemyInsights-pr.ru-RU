---
title: Ограничение доступа в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700468"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничение доступа в SharePoint или OneDrive

Существует множество способов ограничения доступа к службам SharePoint Online и OneDrive. Ниже приведено несколько способов ограничения доступа. 

**Ограничение разрешений**

В SharePoint Online и OneDrive для бизнеса мы ограничен доступ к элементам, таким как сайты, файлы и папки, только предоставляя доступ только тем группам и пользователям, у которых есть доступ.

- [Настройка разрешений для списка или библиотеки SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настройка разрешений сайта в SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Изменение разрешений для вложенной папки](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Управление доступом с неуправляемых устройств](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Как SharePoint или глобальный администратор вы можете заблокировать или ограничить доступ к контенту SharePoint и OneDrive с неуправляемых устройств (не из-за гибридной службы AD или соответствующей возможности в Intune).

**Ограничение расположения в сети**

Администратор ИТ-администраторов может управлять доступом к ресурсам SharePoint и OneDrive на основе определенных сетевых расположений, которым вы доверяете. то есть настроив политику на основе расположения. Дополнительные сведения см. в статье [Управление доступом к данным SharePoint Online и OneDrive в зависимости от расположения в сети](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение блокировки сайта** 

В SharePoint Online вы можете заблокировать семейство веб-сайтов, поэтому доступ к нему у него нет. Это задается с помощью PowerShell и [командной консоли SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощью свойства [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Запретить пользователям создавать сайты или дочерние сайты**

Администратор SharePoint или глобальный администратор могут позволить пользователям создавать и администрировать собственные сайты SharePoint, определять типы сайтов, которые они могут создавать, и указывать расположение сайтов. Дополнительные сведения см. в статье [Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)


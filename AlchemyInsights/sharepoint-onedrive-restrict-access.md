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
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093853"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ограничение доступа в SharePoint или OneDrive

Существует множество способов ограничения доступа к SharePoint online/OneDrive службам. Эти различные методы ограничения доступа описаны ниже. 

**Ограничение разрешений**

В SharePoint Интернете и OneDrive для бизнеса мы ограничим доступ к таким объектам, как сайты, файлы и папки, только тем группам и отдельным лицам, которые должны иметь доступ.

- [Настройка разрешений для списка SharePoint или библиотеки](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Настройка разрешений сайта в SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Изменение разрешений для вложенной папки](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Управление доступом с неуправляемых устройств](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Как администратор SharePoint или глобального администратора, вы можете заблокировать или ограничить доступ к контенту SharePoint и OneDrive с неугодными устройствами (не присоединенными или совместимыми с гибридной AD в Intune).

**Ограничение расположения сети**

Как ИТ-администратор вы можете управлять доступом к SharePoint и OneDrive на основе определенных расположений сети, которые вы доверяете. то есть настроив политику на основе расположения. Дополнительные сведения см. в [веб-сайте Control access to SharePoint Online и OneDrive в зависимости от расположения сети.](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ограничение блокировки сайта** 

В SharePoint Online у вас есть возможность заблокировать коллекцию сайтов, поэтому никто не имеет доступа. Этот набор устанавливается с помощью PowerShell и [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) с помощью свойства [Set-SPOSite-LockState.](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)

**Запретить пользователям создавать сайты или подвиды**

Как администратор SharePoint или глобальный администратор, вы можете позволить пользователям создавать и администрировать собственные сайты SharePoint, определять, какие сайты они могут создавать, и указать расположение сайтов. Дополнительные сведения см. в [веб-сайте Управление созданием сайтов в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)


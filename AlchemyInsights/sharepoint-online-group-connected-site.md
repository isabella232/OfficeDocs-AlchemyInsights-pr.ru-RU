---
title: Добавление группы на сайт SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719494"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Создание сайта, подключенного к группе, в SharePoint Online

<p><strong>При создании или повторном создании подключенного к группе сайта возникла пара распространенных проблем.&nbsp;</strong></p>  <p>1.Если вы удалили группу и подключенный сайт и хотите создать другой сайт с тем же URL-адресом, необходимо удалить предыдущий сайт без возможности восстановления.</p>  <ul>  <li>Загрузка <a title="командной консоли SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Командная консоль</a> - SPO для получения дополнительных сведений о начале работы с PowerShell <a title="см в статье Начало работы с помощью командной консоли SharePoint Online" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Начало работы с консолью</a>управления SharePoint Online. <br /><br /></li>  <li>Удаление сайта из удаленных сайтов с помощью <a title="Remove-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Командлет Remove</a> – SPODeletedSite PowerShell.</li>  </ul>  <p>Если вы создаете сайт, подключенный к группе, и получаете предупреждение <strong>"еще одна группа с таким псевдонимом уже существует"</strong>, проверьте существующие группы <a title="из центра администрирования Office 365." href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 из центра</a>администрирования. Чтобы устранить эту проблему, удалите существующую группу, если она больше не нужна, или создайте сайт с другим назначенным псевдонимом.&nbsp;</p>  <p><strong>Существуют различные способы создания и использования современных групп с SharePoint.&nbsp;</strong></p>  <ol>  <li>Вы можете подключить существующие сайты к группе Office 365. Для получения дополнительных сведений обратитесь <a title="к разделу Подключение группы Office 365 с помощью пользователя SharePoint инетерфаце" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Подключите группу Office 365 с помощью пользователя SharePoint инетерфаце</a>.</li>  <li>Чтобы создать сайт, подключенный к группе Office 365, необходимо создать сайт группы. Дополнительные сведения см <a title=". в статье Создание сайта группы в SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Создайте сайт группы в SharePoint.</a></li>  </ol>


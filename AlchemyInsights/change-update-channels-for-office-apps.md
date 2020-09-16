---
title: Изменение каналов обновления для приложений Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 70b416e2b572fe9b4257648e3426b4d36975681e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756512"
---
# <a name="change-update-channels-for-office-apps"></a>Изменение каналов обновления для приложений Office

Для новых экземпляров Office используйте параметры скачивания программного обеспечения Office, чтобы выбрать нужный канал обновления, а затем установите (или переустановите) приложения Office. Подробнее см. в статье [Управление параметрами скачивания программного обеспечения в Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Примечание** Выбор канала обновления, сделанный с помощью параметров скачивания программного обеспечения Office, действителен для всех пользователей, выполняющих новую установку с помощью портала Office 365. Подробнее см. [Скачивание, установка и переустановка Microsoft 365 или Office 2019 на ПК или Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Чтобы перейти на другой канал обновления для существующих экземпляров Office, используйте средство развертывания Office (ODT).  

1. Скачайте последнюю версию средства ODT (setup.exe) в [Центре загрузки Майкрософт](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Укажите имя канала, на который вы хотите переключиться. Дополнительные сведения см. в статье [Параметры конфигурации для средства развертывания Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Создайте конфигурационный XML-файл, указав название соответствующего канала, например update.xml.  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. Из командной строки для администратора перейдите в папку, где расположен файл setup.exe, и введите следующую команду:  
    а. setup.exe /configure update.xml
5. Запустите приложение Office (например, Excel), а затем щелкните **Файл** > **Учетная запись**. В разделе "Сведения о продукте" выберите **Параметры обновления** > **Обновить сейчас**.

Подробнее см. в статье [Как перейти на другой канал обновления для существующих приложений Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Чтобы переключиться на канал обновления для выбранной группы пользователей или с помощью диспетчера конфигураций (SCCM), настройте параметр канала обновления с помощью GPO. Дополнительные сведения см. в статье [Обзор каналов обновления для Приложений Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Подробнее см. в статье [Как управлять каналами Office 365 профессиональный плюс для ИТ-специалистов](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) и [Как управлять обновлениями Приложений Microsoft 365 с помощью Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).
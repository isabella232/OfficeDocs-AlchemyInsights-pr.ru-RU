---
title: Управление автоматическими обновлениями приложений Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747789"
---
# <a name="control-automatic-updates-for-office-apps"></a>Управление автоматическими обновлениями приложений Office

По умолчанию обновления для приложений Office загружаются автоматически и применяются в фоновом режиме, без какого-либо вмешательства со стороны пользователя. При этом администраторы могут управлять порядком применения обновлений с помощью параметров обновления Office. С помощью параметров обновления администраторы могут включать и отключать автоматическое обновление, отображать или скрывать кнопку **Обновить сейчас** в Office, устанавливать крайние сроки обновлений и выполнять другие действия. Подробные сведения см. в следующих статьях:

- [Настройка параметров обновления для Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Автоматическое обновление для Office не включено](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Определение способа обновления Office после установки](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Чтобы проверить существующие параметры обновления, примененные к клиентскому компьютеру, выполните следующие действия:

1. Откройте редактор реестра: нажмите кнопку **Пуск** > **Выполнить** > **regedit**.
2. Перейдите в следующее расположение и проверьте параметры обновления Office:  
    а. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Примечание**. Если задан раздел реестра OfficeMgmtCOM, в окне **Office** > **Учетная запись** > **Обновления Office** может отображаться сообщение "Обновлениями управляет системный администратор". Дополнительные сведения см. в статье [Управление обновлениями для Приложений Microsoft 365 с помощью Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  
---
title: Устранение неполадок при синхронизации паролей
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387890"
---
# <a name="troubleshoot-password-synchronization"></a>Устранение неполадок при синхронизации паролей

Чтобы устранить проблемы с синхронизацией паролей, начните с использования этой задачи по устранению неполадок подключения AAD, чтобы определить причину, по которой не синхронизируются пароли. Чтобы начать, перейдите к разделу [Управление прямой синхронизацией](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Откройте новый сеанс Windows PowerShell на сервере Azure AD Connect и выберите пункт **Запуск от имени администратора** .

2. Выполните командлет Set — ExecutionPolicy RemoteSigned или Set/ExecutionPolicy Unrestricted.

3. Запустите мастер Azure AD Connect.

4. Перейдите на страницу дополнительные задачи > " **Устранение неполадок**"  >  **Next**.

5. Нажмите кнопку **запустить** , чтобы открыть меню устранение неполадок PowerShell.

6. Выберите пункт **Устранение неполадок при синхронизации паролей**.

    Эта ошибка обычно заключается в том, что пароль не синхронизируется для конкретной учетной записи пользователя.

    **Примечания** Если время последней успешной синхронизации пароля прошло некоторое время, синхронизация паролей завершается с ошибкой назад.

Дополнительные сведения об устранении неполадок при синхронизации паролей приведены [в статье Устранение неполадок синхронизации паролей с помощью Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).
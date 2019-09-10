---
title: Перемещение сообщений электронной почты в архивный почтовый ящик
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822175"
---
# <a name="move-email-to-the-archive-mailbox"></a>Перемещение электронной почты в архивный почтовый ящик

1. Убедитесь, что **архивный почтовый ящик** включен. В противном случае выполните действия, описанные в [этой статье](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , чтобы включить архивный почтовый ящик.

2. Чтобы автоматически архивировать сообщения в архивный почтовый ящик, тег хранения с действием **переместить в архив** должен **автоматически применять ко всему тегу почтового ящика (по умолчанию)**. Выполните действия, описанные в этой статье, чтобы создать тег: [Archive Default Tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Затем добавьте тег **Archive** в политику хранения. В центре администрирования Exchange выберите **политики хранения** > добавить **тег "переместить в архив** " в политику > **сохранить**.

4. Теперь [назначьте политику хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) для почтового ящика определенного пользователя. Та же политика будет применяться и к **основному** , и к **архивному** почтовому ящику.

Может потребоваться принудительно запустить помощник по обслуживанию управляемых папок (MFA) и применить новые параметры к почтовому ящику пользователя. Выполните следующую команду при [подключении к EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) для запуска помощника по работе с управляемыми папками для определенного почтового ящика:
  
Start — ManagedFolderAssistant — Identity<name of the mailbox>

Дополнительные сведения о настройке политики архивации можно найти в разделе [Настройка политики архивации и удаления для почтовых ящиков](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  
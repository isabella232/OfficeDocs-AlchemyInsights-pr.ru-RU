---
title: Перемещение сообщений электронной почты в почтовый ящик Archive
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974970"
---
# <a name="move-email-to-the-archive-mailbox"></a>Перемещение электронной почты в почтовый ящик архива

Если вы хотите, чтобы мы запускали автоматические проверки указанных ниже параметров, выберите кнопку < -- в верхней части этой страницы, а затем введите адрес электронной почты пользователя, у которого возникли проблемы с перемещением электронной почты в архивный почтовый ящик.

1. Подтверждение включения **архивного почтового** ящика. Если нет, используйте шаги в [этой статье,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) чтобы включить почтовый ящик архива.

2. Чтобы автоматически архивировать сообщения в архивном почтовом ящике, необходимо установить тег хранения с действием **Move to archive,** который должен автоматически применяться к всему тегу почтового ящика **(по умолчанию).** Используйте здесь шаги для создания тега: [тег Архив по умолчанию](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Затем добавьте тег **Archive** в политику хранения. В центре администрирования Exchange выберите  политики хранения > добавить тег **Move to Archive** в > **Сохранить**.

4. Теперь [назначьте политику хранения](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) в почтовый ящик конкретного пользователя. Такая же политика будет применяться  как к основному, так и к почтовому **ящику Archive.**

Может потребоваться заставить помощника по управляемой папке (MFA) запускать и применять новые параметры к почтовому ящику пользователя. Запустите следующую команду, [подключенную к EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) чтобы запустить помощник управляемых папок для определенного почтового ящика:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Дополнительные сведения о настройке политики архива см. в статью Настройка политики архива и удаления [для почтовых ящиков.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  
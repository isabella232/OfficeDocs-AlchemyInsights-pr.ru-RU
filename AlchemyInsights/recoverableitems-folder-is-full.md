---
title: Папка 1336 RecoverableItems заполнена
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061769"
---
# <a name="the-recoverable-items-folder-is-full"></a>Папка "Извлекаемые элементы" заполнена

Для Exchange Online почтовых ящиков ограничение хранения по умолчанию для папки "Извлекаемые элементы" составляет 30 ГБ. Ограничение хранилища для папки "Извлекаемые элементы" автоматически увеличивается до 100 ГБ, если почтовый ящик размещен на удержании судебного разбирательства, удержании электронных данных или назначен политике хранения.

Когда папка "Извлекаемые элементы" достигает предельного уровня хранения, на функциональность почтовых ящиков влияют следующие способы:

- Пользователь не может удалять элементы из почтового ящика.

- Помощник для управляемых папок не может удалять элементы на основе тега хранения или параметров управляемых папок.

- Для почтовых ящиков, в которые включено или отложено восстановление одного элемента, процесс защиты страниц с копированием на записи не может поддерживать версии элементов, редактируемого пользователем.

- Для почтовых ящиков с включенной регистрацией аудита почтовых ящиков записи журналов аудита почтовых ящиков не могут быть сохранены в подвездной папке Аудиты в папке "Извлекаемые элементы".

Для почтовых ящиков, которые не на удержании, администраторы могут использовать команду в Exchange Online PowerShell для удаления элементов в папке `Search-Mailbox -SearchDumpsterOnly -DeleteContent` "Извлекаемые элементы". Дополнительную информацию см. в следующих статьях:

- [Поиск и удаление сообщений](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Для почтовых ящиков, которые находятся в удержании, администраторам необходимо удалить удержание, прежде чем они смогут удалить элементы из папки "Извлекаемые элементы". Дополнительные сведения см. в публикации [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Чтобы предотвратить заполнение папки "Извлекаемые элементы", администраторы могут увеличить ограничение хранения папки "Извлекаемые элементы" для почтовых ящиков на удержание и настроить политику хранения почтовых ящиков, которая перемещает элементы из папки "Извлекаемые элементы" в архивный почтовый ящик пользователя. См. [увеличение квоты извлекаемых элементов для почтовых ящиков в удержании.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)

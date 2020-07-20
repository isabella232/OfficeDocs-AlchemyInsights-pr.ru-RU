---
title: Проблема при открытии и скачивании файлов в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146819"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Проблема при открытии и скачивании файлов в Yammer

Классическая версия Yammer поддерживает несколько вариантов передачи файлов в сообщения и группы. В зависимости от конфигурации сети файлы по умолчанию хранятся в SharePoint.

Средство выбора файлов в новой версии Yammer пока что поддерживает не все варианты, доступные в классической версии Yammer. В последующих обновлениях будут добавлены дополнительные возможности. Дополнительные сведения см. в статье [Вложение файла или изображения в сообщение беседы Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Не удается открыть или скачать файл**  

Файл можно передать в Yammer, но также связан с файлом в SharePoint Online. Чтобы устранить проблему, сначала необходимо определить расположение файла. У файла, переданного в Yammer, будет URL-адрес *.yammer.com. Убедитесь в том, что необходимые URL-адреса и IP-адреса не заблокированы. Дополнительные сведения см. в записи блога [Использование жестко закодированных IP-адресов для Yammer не рекомендуется](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Выясните, может ли пользователь с правами глобального администратора скачать файл. Если файл является частным, может потребоваться использовать режим личного контента. Дополнительные сведения см. в статье [Отслеживание личного контента в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Гости и файлы на уровне сети Yammer в SharePoint Online**  

[Гости на уровне сети в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не используют Azure AD B2B и являются внутренними по отношению к службе Yammer, поэтому они не могут получить доступ к файлам Yammer, хранящимся в SharePoint. Создайте внешнего пользователя AAD B2B, который сможет получать доступ к библиотекам документов в SharePoint Online с помощью этого удостоверения. Сведения о будущей поддержке гостей Azure AD B2B в Yammer см. в статье [Поддержка гостевых пользователей сегмента бизнес-бизнес (B2B) в предварительной версии Yammer: Условия для клиентов и часто задаваемые вопросы](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).
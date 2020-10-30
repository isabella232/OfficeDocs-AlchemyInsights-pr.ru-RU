---
title: Устранение проблем с защитником Microsoft для Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801420"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Устранение неполадок, связанных с Office 365 ATP

- **Задержки при доставке сообщений электронной почты** ? Попробуйте использовать параметр динамической доставки для политик безопасных вложений ATP. Это не позволит задержкам доставки сообщений электронной почты при защите получателей от вредоносных файлов.
- **Хотите ли вы сообщить о ложных срабатываниях или ложных отрицательные отрицательные** результаты? Используйте эту ссылку, чтобы передать файл для анализа: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Знаете ли вы, что вы можете включить защиту для безопасных ссылок ATP для электронной почты, отправляемой между людьми в Организации** ? Выполните следующие действия:
    1. Перейдите к разделу https://protection.office.com и войдите в систему.
    2. Перейдите к **Threat management** разделу  >  **Policy**  >  **безопасные ссылки** политики управления угрозами.
    3. В разделе **политики, которые применяются к определенным получателям** , измените (или добавьте) политику.
    4. Выберите **Применить безопасные ссылки к сообщениям, отправляемым в Организации** .
    5. Сохраните политику и разрешите около 30 минут, чтобы изменения работали в центре обработки данных.
- Для получения дополнительной справки по ATP обратитесь к разделу [защитник Майкрософт для Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).
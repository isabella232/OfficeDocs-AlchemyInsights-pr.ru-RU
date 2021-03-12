---
title: Устранение неполадок при установке MDATP на Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737661"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Устранение неполадок при установке MDATP на Mac

Если не удается установить вручную, на странице **Сводка** мастера установки показано следующее:

"Ошибка произошла во время установки. Установщик столкнулся с ошибкой, из-за которой установка не справилась с работой. Обратитесь за помощью к производителю программного обеспечения".

Для развертывания MDM на странице также показан общий сбой установки.

Хотя мы не отображаем точные ошибки конечным пользователям, мы храним файл журнала с ходом установки в **/Library/Logs/Microsoft/mdatp/install.log**. Каждый сеанс установки примыкает к этому файлу журнала. Для вывода последнего сеанса установки используйте `sed` .

Дополнительные новости см. в выпуске Проблемы с установкой устранения неполадок [для MICROSOFT Defender ATP для Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)

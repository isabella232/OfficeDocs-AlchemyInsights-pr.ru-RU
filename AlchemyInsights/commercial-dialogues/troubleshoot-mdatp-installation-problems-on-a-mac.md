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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091072"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Устранение неполадок при установке MDATP на Mac

Если не удается установить вручную, на странице **Сводка** мастера установки показано следующее:

"Ошибка произошла во время установки. Установщик столкнулся с ошибкой, из-за которой установка не справилась с работой. Обратитесь за помощью к производителю программного обеспечения".

Для развертывания MDM на странице также показан общий сбой установки.

Хотя мы не отображаем точные ошибки конечным пользователям, мы храним файл журнала с ходом установки в **/Library/Logs/Microsoft/mdatp/install.log**. Каждый сеанс установки примыкает к этому файлу журнала. Для вывода последнего сеанса установки используйте `sed` .

Дополнительные новости см. в выпуске Проблемы с установкой устранения неполадок [для MICROSOFT Defender ATP для Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)

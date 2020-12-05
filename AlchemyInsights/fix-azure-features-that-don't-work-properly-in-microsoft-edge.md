---
title: Что делать, если функции Azure не работают должным образом в Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576598"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Что делать, если функции Azure не работают должным образом в Microsoft Edge

Microsoft Edge имеет [Известные проблемы](https://go.microsoft.com/fwlink/?linkid=2140608) , связанные с зонами безопасности, и может повлиять на то, как пользователи Azure входят в центр администрирования Windows. Если у вас возникли проблемы с использованием функций Azure с Microsoft EDGE, попробуйте выполнить следующие действия:

1. В меню **Пуск** выберите пункт **Свойства браузера** и выберите его.
2. В диалоговом окне **Свойства обозревателя** перейдите на вкладку **Безопасность** .
3. Выберите зону **Надежные сайты** , а затем нажмите кнопку **сайты** .
4. В диалоговом окне **Надежные сайты** добавьте URL-адрес шлюза, а также [https://login.microsoftonline.com](https://login.microsoftonline.com) и нажмите [https://login.live.com](https://login.live.com) кнопку **Закрыть**.
5. В диалоговом окне **Свойства обозревателя** перейдите на вкладку **Конфиденциальность** .
6. В разделе **блокирование всплывающих окон** выберите **Параметры**. В открывшемся диалоговом окне Добавьте URL-адрес шлюза, а также [https://login.microsoftonline.com](https://login.microsoftonline.com) и нажмите [https://login.live.com](https://login.live.com) кнопку **Закрыть**.

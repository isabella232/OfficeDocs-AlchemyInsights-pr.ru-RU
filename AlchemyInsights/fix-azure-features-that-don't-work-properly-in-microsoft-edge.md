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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117101"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Что делать, если функции Azure не работают должным образом в Microsoft Edge

Microsoft Edge имеет [известные](https://go.microsoft.com/fwlink/?linkid=2140608) проблемы, связанные с зонами безопасности, и может повлиять на то, как пользователи Azure войдите в Windows Центр администрирования. Если у вас возникли проблемы с использованием функций Azure с Microsoft Edge, попробуйте следующие действия:

1. В меню **Пуск** выберите **параметры Интернета** и выберите его.
2. В **диалоговом окне Свойства** Интернета перейдите на вкладку **Security.**
3. Выберите **зону доверенных сайтов** и выберите **кнопку "Сайты".**
4. В **диалоговом окне Доверенные** сайты добавьте URL-адрес шлюза, а [https://login.microsoftonline.com](https://login.microsoftonline.com) также и выберите [https://login.live.com](https://login.live.com) **Закрыть**.
5. В **диалоговом окне Свойства** Интернета перейдите на вкладку **Конфиденциальность.**
6. В разделе **Всплывающий блокатор** выберите **Параметры**. В открываемом диалоговом окне добавьте URL-адрес шлюза, а затем выберите [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) **Close**.

---
title: Что делать, если функции Azure не работают должным образом в Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950326"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Что делать, если функции Azure не работают должным образом в Microsoft Edge

В Microsoft Edge есть известные проблемы, связанные с зонами безопасности, которые могут влиять на вход пользователей Azure в Windows Admin Center. Дополнительные сведения см. в статье [Известные проблемы в Microsoft Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Если у вас возникли проблемы с использованием функций Azure в Microsoft Edge, попробуйте выполнить следующие действия.

1. В меню "Пуск" на панели **поиска** введите **свойства браузера** и выберите этот результат.
1. В разделе **Свойства: Интернет** выберите вкладку **Безопасность**.
1. Выберите **Надежные сайты**, а затем нажмите **Сайты**.
1. Добавьте URL-адрес своего шлюза, а также <https://login.microsoftonline.com> и <https://login.live.com>. После этого нажмите **Закрыть**.
1. В разделе **Свойства: Интернет** выберите вкладку **Конфиденциальность**.
1. В разделе "Блокирование всплывающих окон" выберите **Параметры**. Добавьте URL-адрес своего шлюза, а также <https://login.microsoftonline.com> и <https://login.live.com>. После этого нажмите **Закрыть**.
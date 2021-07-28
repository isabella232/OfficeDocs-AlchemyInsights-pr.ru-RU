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
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603294"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Что делать, если функции Azure не работают должным образом в Microsoft Edge

В Microsoft Edge есть известные проблемы, связанные с зонами безопасности, которые могут влиять на вход пользователей Azure в Windows Admin Center. Дополнительные сведения см. в статье [Известные проблемы в Microsoft Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Если у вас возникли проблемы с использованием функций Azure в Microsoft Edge, попробуйте выполнить следующие действия.

1. В меню "Пуск" на панели **поиска** введите **свойства браузера** и выберите этот результат.
1. В разделе **Свойства: Интернет** выберите вкладку **Безопасность**.
1. Выберите **Надежные сайты**, а затем нажмите **Сайты**.
1. Добавьте URL-адрес своего шлюза, а также <https://login.microsoftonline.com> и <https://login.live.com>. После этого нажмите **Закрыть**.
1. В разделе **Свойства: Интернет** выберите вкладку **Конфиденциальность**.
1. В разделе "Блокирование всплывающих окон" выберите **Параметры**. Добавьте URL-адрес своего шлюза, а также <https://login.microsoftonline.com> и <https://login.live.com>. После этого нажмите **Закрыть**.
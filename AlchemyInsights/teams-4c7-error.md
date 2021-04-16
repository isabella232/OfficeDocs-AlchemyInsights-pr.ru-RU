---
title: Ошибка Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786682"
---
# <a name="4c7-error-in-microsoft-teams"></a>Ошибка 4c7 в Microsoft Teams

Эта ошибка возникает из-за того, что Microsoft Teams требует проверки подлинности форм. При развертывании служб Федерации Active Directory (AD FS) проверка подлинности форм не включена для интрасети по умолчанию. Если сбой в интегрированной проверке подлинности Windows, вам будет предложено войти с помощью проверки подлинности форм.

Чтобы устранить эту проблему, введи проверку подлинности форм с помощью оснастки AD FS Microsoft Management Console (MMC) на компьютере с локальной копией Active Directory. Для этого выполните следующие действия: 

1. В области навигации просмотрите политики **проверки подлинности.**
2. В **области Действия** в области сведений выберите Изменить **глобальную первичную проверку подлинности.**
3. На **вкладке Intranet** выберите **проверку подлинности форм.**
4. Выберите **ОК** (или **Применить).**
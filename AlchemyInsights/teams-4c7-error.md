---
title: Teams 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049321"
---
# <a name="4c7-error-in-microsoft-teams"></a>Ошибка 4c7 в Microsoft Teams

Эта ошибка возникает, Microsoft Teams требуется проверка подлинности форм. При развертывании служб Федерации Active Directory (AD FS) проверка подлинности форм не включена для интрасети по умолчанию. Если Windows сбой комплексной проверки подлинности, вам будет предложено войти с помощью проверки подлинности форм.

Чтобы устранить эту проблему, введи проверку подлинности форм с помощью оснастки AD FS Microsoft Management Console (MMC) на компьютере с локальной копией Active Directory. Для этого выполните следующие действия: 

1. В области навигации просмотрите политики **проверки подлинности.**
2. В **области Действия** в области сведений выберите Изменить **глобальную первичную проверку подлинности.**
3. На **вкладке Intranet** выберите **проверку подлинности форм.**
4. Выберите **ОК** (или **Применить).**
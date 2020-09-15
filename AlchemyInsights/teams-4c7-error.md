---
title: Ошибка 4c7 Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700216"
---
# <a name="4c7-error-in-microsoft-teams"></a>Ошибка 4c7 в Microsoft Teams

Эта ошибка возникает, потому что для Microsoft Teams требуется проверка подлинности на формах. При развертывании служб федерации Active Directory (AD FS) проверка подлинности по умолчанию для интрасети по умолчанию отключена. Если произойдет сбой встроенной проверки подлинности Windows, вам будет предложено выполнить вход с использованием проверки подлинности на основе форм.

Чтобы устранить эту проблему, включите проверку подлинности на основе форм с помощью оснастки консоли управления (MMC) AD FS на компьютере с локальной копией Active Directory. Для этого выполните следующие действия: 

1. В области навигации перейдите к **политикам проверки подлинности**.
2. В разделе **действия** в области сведений выберите **изменить глобальную основную проверку подлинности**.
3. На вкладке **интрасеть** выберите **Проверка подлинности с помощью форм**.
4. Нажмите кнопку **ОК** (или **Применить**).
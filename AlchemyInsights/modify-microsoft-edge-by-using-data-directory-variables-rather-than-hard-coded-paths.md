---
title: Изменение Microsoft Edge с помощью переменных каталога данных, а не жестко заданных путей
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992304"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Изменение Microsoft Edge с помощью переменных каталога данных, а не жестко заданных путей

Например, чтобы в Windows сохранить данные профиля в локальных данных приложения пользователя, а не в расположении по умолчанию, установите для политики *UserDataDir* значение **${local_app_data}\Edge\Profile**.

Дополнительные сведения см. в статье [Создание переменных каталога пользовательских данных Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).
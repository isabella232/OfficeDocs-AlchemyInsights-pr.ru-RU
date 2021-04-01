---
title: Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве, присоединенном к домену
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426894"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Настройка Microsoft Edge в качестве браузера по умолчанию на устройстве, присоединенном к домену

Настройка Microsoft Edge в качестве браузера по умолчанию 

1. [Создайте файл конфигурации связей по умолчанию](https://go.microsoft.com/fwlink/?linkid=2132437) и сохраните его локально или в сетевой папке.

1. Откройте редактор групповой политики и перейдите в **Конфигурация компьютера** > **Административные шаблоны** > **Компоненты Windows** > **Проводник**.

1. Выберите **Установить файл связей по умолчанию**.

1. Выберите **Установка параметров конфиденциальности** и нажмите **Вкл.**.

1. В разделе **Параметры** введите расположение файла конфигурации связей по умолчанию, а затем выберите **ОК**.

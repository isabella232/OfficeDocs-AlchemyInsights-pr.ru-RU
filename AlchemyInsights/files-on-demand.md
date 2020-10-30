---
title: Файлы по запросу
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791307"
---
# <a name="configure-files-on-demand"></a>Настройка функции "Файлы по запросу"

Для работы функции "Файлы из OneDrive по запросу" требуются [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (версии 1709 или более поздней) или Windows Server 2019 и OneDrive сборки 17.3.7064.1005 или более поздней.

Функция "Файлы из OneDrive по запросу" позволяет получать доступ к файлам в OneDrive, не скачивая их все на свое устройство.

Чтобы настроить функцию "Файлы по запросу" на своем компьютере, выполните указанные ниже действия.

1. Щелкните белый или синий значок облака **OneDrive** в области уведомлений на панели задач Windows. Нажмите значок шестеренки **Справка и параметры** > **Параметры** .
2. На вкладке **Параметры** установите флажок **Экономить место, скачивая файлы по мере необходимости** .  

Вы также можете настроить функцию "Файлы по запросу" с помощью реестра.

Если вы отключите этот параметр, процедура синхронизации для пользователей Windows 10 будет той же, что и для пользователей предыдущих версий Windows, и они не смогут включить функцию "Файлы по запросу". Если вы не настраиваете этот параметр, пользователи могут включать и отключать функцию "Файлы по запросу".

Включение этой политики устанавливает значение 1 для следующего раздела реестра: Выключение этой политики устанавливает значение 0 для следующего раздела реестра:

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Если вы не видите параметра "Файлы по запросу" в разделе "Параметры", убедитесь в том, что тип запуска "Windows Cloud Files Filter Driver" имеет значение 2 (AUTO_START). При включении этой функции устанавливается значение 2 для следующего раздела реестра:

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`
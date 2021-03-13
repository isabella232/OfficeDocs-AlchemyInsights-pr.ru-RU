---
title: Удаление фоновой службы Поиска (Майкрософт) в Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753442"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Удаление фоновой службы Поиска (Майкрософт) в Bing

Чтобы удалить фоновую службу Поиска (Майкрософт) в Bing, попробуйте следующие решения.

1. Чтобы вернуться к исходным настройкам поисковой системы, выполните следующие действия.

    а. Переведите переключатель **Использовать Bing в качестве поисковой системы по умолчанию[ в положение](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)Выкл**.

    б. [Перейдите в Центр администрирования Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) и снимите флажок с параметра, влияющего на всех пользователей в организации.

2. Чтобы удалить фоновую службу с отдельного устройства, выполните следующие действия.

    а. Выберите **Панель управления > Программы > Программы и компоненты**.

    б. Щелкните правой кнопкой мыши **Поиск (Майкрософт) в Bing** в списке установленных программ и нажмите **Удалить**.

3. Чтобы удалить фоновую службу с нескольких устройств в организации, войдите в систему с учетной записью администратора и запустите следующую команду в сценарии. 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`

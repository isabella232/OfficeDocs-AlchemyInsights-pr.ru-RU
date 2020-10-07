---
title: Развертывание приложений Win32 с помощью Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366528"
---
# <a name="intune-win32-app-deployment"></a>Развертывание приложений Win32 с помощью Intune

Microsoft Intune дает возможность развертывать приложения Win32, включая MSI и EXE, на устройствах с Windows 10. Для механизма развертывания требуется, чтобы на целевом устройстве было расширение управления Intune (IME). Расширение IME устанавливается автоматически, если нацелить сценарий PowerShell или развертывание приложения Win32 на определенного пользователя или устройство.

Для развертывания приложений Win32 также необходимо выполнить ряд предварительных требований:

- Поддерживаемые платформы: Windows 10 версии 1607 или более поздней (Корпоративная, Pro и для образовательных учреждений).
- Поддерживаемые архитектуры: x86 и x64.
- Управление устройствами: требуется присоединение к AAD и автоматическая регистрация (включая присоединение к гибридному домену и автоматическая регистрация с помощью групповой политики).
- Формат пакета приложения: файл с расширением.**intunewin**, подготовленный с помощью [средства подготовки содержимого Win32 (Майкрософт)](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Ограничения:
    - Максимальный размер: 8 ГБ.
    - Неподдерживаемая архитектура: ARM.

Прочтите документ "[Добавление, назначение и мониторинг приложений Win32 в Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" для получения сведений, связанных с этими действиями.

Сведения об устранении неполадок при развертывании приложений в Windows, включая приложения Win32, см. в следующих документах:

- [Устранение неполадок при установке приложений](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Устранение неполадок приложений Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)
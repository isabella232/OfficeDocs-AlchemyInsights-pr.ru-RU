---
title: Проблемы при установке Microsoft Defender на Mac и Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325262"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблемы при установке Microsoft Defender на Mac и Linux

**Mac**

- Перед установкой пакета Microsoft Defender для Mac убедитесь, что система удовлетворяет требованиям. Дополнительные сведения см. в статье [Установка Microsoft Defender для Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Ознакомьтесь со сведениями в файле "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Перед установкой пакета Microsoft Defender ATP для Linux убедитесь, что система удовлетворяет требованиям. Дополнительные сведения см. в статье [Установка MDATP для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Чтобы узнать, как проверить, запущена ли служба MDATP, ознакомьтесь с разделом [Сбой установки](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Если службу запустить не удалось, то, чтобы найти и устранить проблемы, следуйте инструкциям в разделе [Действия по устранению неполадок, если служба MDATP не запущена](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Пошаговые инструкции по проверке конфигурации клиента, которые помогут проверить состояние продукта и прогнать тест для обнаружения неполадок с помощью текстового файла EICAR, см. в разделе [Конфигурация клиента](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Примечание.** Список файловых систем, для которых поддерживается управление доступом, см. в статье [ATP в Microsoft Defender для Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).
---
title: Действия Защитника Windows в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: af9e8e16fe96b7460b19481900e4c46d0a2a27f73293f81b5af86131af40287a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047377"
---
# <a name="windows-defender-actions-in-intune"></a>Действия Защитника Windows в Intune

Можно использовать Intune, чтобы запускать проверку по запросу и обновлять сигнатуры вирусов в Защитнике Windows на отдельных устройствах.

После успешного запуска удаленного действия это действие записывается в журнале событий Защитника Windows.

Политика Windows Endpoint Protection дает возможность создавать в Intune дополнительные параметры для функций Защитника Windows и применять их к наборам устройств.

Дополнительные сведения о запуске действий Защитника Windows см. в статье [Настройка и запуск проверки антивирусной программы в Microsoft Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).
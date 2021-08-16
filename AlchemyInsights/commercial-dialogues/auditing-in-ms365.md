---
title: Аудит в Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: a5acd322186f8f4b7734f8541877a642a553288e10b3c122e4f276b9bb611308
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988986"
---
# <a name="auditing-in-microsoft-365"></a>Аудит в Microsoft 365

Вот несколько вещей, которые необходимо знать о аудите в Microsoft 365:

1. Exchange по умолчанию проверяются действия администратора.
1. Мы по умолчанию включаем аудит почтовых ящиков для всех пользователей. Чтобы узнать больше об этом, нажмите [здесь](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171). До этого момента, если вы хотите, чтобы инструкции вручную включить его для одного человека или всей организации, выберите кнопку Включив аудит почтовых ящиков ниже.
1. Microsoft 365 Почтовые ящики групп и почтовые ящики общедоступных папок не поддерживают ведение журнала аудита.
1. Для SharePoint/OneDrive не требуется дополнительная конфигурация для включенного аудита. Чтобы узнать, какие действия проверяются, см. в этой информации:
    1. [Действия файла](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Действия, связанные с папками](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Действия по совместному доступу и совместному доступу.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
1. Список всех проверенных действий службы см. в [перечне проверенных действий.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)

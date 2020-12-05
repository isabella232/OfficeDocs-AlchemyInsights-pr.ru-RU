---
title: Значок календаря не отображается в клиенте Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576621"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Значок календаря не отображается в клиенте Microsoft Teams

Для работы с вкладкой **Календарь** в Teams требуется доступ к почтовому ящику Exchange через веб-службы Exchange. Почтовый ящик Exchange может быть подключен к сети или локальной среде. Для пользователей Online, которые не видят вкладку **Календарь** , убедитесь, что они [лицензированы для почтового ящика Exchange Online, а почтовый ящик включен](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Если пользователи размещены в локальной среде, необходимо подтвердить работоспособность гибридной конфигурации. Используйте [мастер гибридной конфигурации](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) для устранения неполадок. Обратите внимание, что [для Teams требуется Exchange 2016 CU3 или выше](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Дополнительные сведения и инструкции по устранению неполадок приведены в разделе [Устранение неполадок взаимодействия Microsoft Teams и Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).

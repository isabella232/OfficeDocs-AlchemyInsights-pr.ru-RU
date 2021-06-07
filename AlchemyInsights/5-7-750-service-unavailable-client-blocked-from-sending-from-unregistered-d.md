---
title: 1048 5.7.750 Служба недоступна. Клиент заблокирован от отправки из незарегистрированных доменов
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774264"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Отправка клиентом из незарегистрированного домена заблокирована

Ошибка возникает, когда большой объем сообщений отправляется из доменов, которые не предусмотрены в клиенте (добавлены в качестве принятых доменов и проверены).

Чтобы избежать этой ошибки, вы можете использовать соединителю потока почты на основе сертификата, где домен сертификата является предварительным доменом, или вы можете укажете все отправляя домены.

Дополнительные сведения см. в статье [Устранение проблем с доставкой электронной почты для кодов ошибок с 5.7.700 по 5.7.750 включительно в Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).
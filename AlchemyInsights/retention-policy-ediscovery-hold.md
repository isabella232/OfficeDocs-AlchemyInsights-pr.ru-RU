---
title: 2609 — хранение и обнаружение электронных данных
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727904"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Не удается удалить элементы в SharePoint Online или OneDrive для бизнеса

Невозможно удалить элементы из SharePoint Online или OneDrive для бизнеса, так как политика хранения, метка хранения или удержание обнаружения электронных данных применяются к сайту SharePoint или определенному элементу. Сюда также не удается удалить документ, версию документа, папку, библиотеку документов, список, приложение, сайт или семейство веб-сайтов. 

Чтобы удалить элементы в одном из этих сценариев, необходимо удалить политику хранения, метку хранения или удержание обнаружения электронных данных (сайт должен быть исключен из политики хранения). Необходимо отключить или исключить соответствующие удержания, которые приводят к возникновению этой проблемы. После удаления политики хранения или удержания может потребоваться до 24 часов, чтобы изменения вступили в силу. 

Сведения о различных функциях хранения и хранения, которые можно применить к сайтам SharePoint и учетным записям OneDrive, можно найти в следующих разделах.

- [Обзор политик хранения](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [Обзор меток хранения](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [Управление удержаниями в Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [удержания электронных данных](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [Политики закрытия и удаления устаревших сайтов](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
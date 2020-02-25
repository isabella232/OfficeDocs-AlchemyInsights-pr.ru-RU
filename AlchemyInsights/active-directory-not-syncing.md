---
title: Active Directory не синхронизируется
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265269"
---
# <a name="active-directory-not-syncing"></a>Active Directory не синхронизируется

При получении сообщений об ошибках синхронизации, например "нет последней синхронизации", или Обратите внимание на состояние синхронизации службы каталогов на портале администрирования Office — сообщение "время последней синхронизации больше 3 дней назад", может быть неправильные параметры AADConnect или недостаточно разрешения для выполнения синхронизации.  

Переустановка AADConnect с помощью Express Settings может ускорить решение проблемы:

1. [Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следуйте инструкциям по установке Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Дополнительные сведения об учетных записях служб AADConnect можно найти в статье [Azure AD Connect: accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

---
title: Active Directory не синхронизируется
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697642"
---
# <a name="active-directory-not-syncing"></a>Active Directory не синхронизируется

При получении сообщений об ошибках синхронизации, например "нет последней синхронизации", или Обратите внимание на состояние синхронизации службы каталогов на портале администрирования Office — сообщение "время последней синхронизации больше трех дней назад", возможно, что у AADConnect есть неправильные параметры или недостаточно разрешений для выполнения синхронизации.  

Переустановка AADConnect с помощью Express Settings может ускорить решение проблемы:

1. [Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следуйте инструкциям по установке Express](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Дополнительные сведения об учетных записях службы AADConnect см. в статье [Azure AD Connect: учетные записи и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

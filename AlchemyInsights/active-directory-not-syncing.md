---
title: Active Directory, не синхронизируются
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314217"
---
# <a name="active-directory-not-syncing"></a>Active Directory, не синхронизируются

Если вы получаете ошибки синхронизации, такие как "не последняя синхронизация", или обратите внимание на состояние синхронизации каталогов на портале администрирования Office: "Последняя синхронизация более 3 дней назад", возможно, AADConnect имеет неправильные параметры или недостаточно разрешений для выполнения синхронизации.  

Переустановка AADConnect с помощью экспресс-параметров может быстро устранить проблему:

1. [Скачайте последнюю версию AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следуйте инструкциям по экспресс-установке.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect необходимо устанавливать в операционной системе Windows Server 2012 или более поздней версии. Этот сервер должен быть присоединен к домену, это может быть как контроллер домена, так и рядовой сервер. Полный список требований и предварительных требований Azure AD Подключение просмотреть необходимые условия для [Azure AD Подключение.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Дополнительные сведения об учетных записях службы AADConnect см. в статье [Azure AD Connect: учетные записи и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).

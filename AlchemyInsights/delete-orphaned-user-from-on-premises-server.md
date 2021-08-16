---
title: Удаление потерянного пользователя из локального сервера
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102278"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Удаление потерянного пользователя из локального сервера

Чтобы удалить потерянного пользователя, выполните указанные ниже действия.

1. Выполните принудительную синхронизацию службы каталогов, следуя инструкциям в статье [Что такое гибридное удостоверение в Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Для подтверждения синхронизации каталогов следуйте инструкциям в статье [Что такое гибридное удостоверение в Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Если функция синхронизации работает должным образом, но удаление объекта Active Directory не переносится в Azure AD, необходимо вручную удалить потерянный объект с помощью одного из следующих командлетов Azure Active Directory для Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Например, чтобы удалить потерянный идентификатор пользователя john.smith@contoso.com, созданный с помощью синхронизации службы каталогов, запустите командлет.

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com
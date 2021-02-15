---
title: Групповая политика
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243920"
---
# <a name="group-policy"></a>Групповая политика

Параметры для объектов пользователей и компьютеров в доменных службах Azure Active Directory (Azure AD DS) часто управляются с помощью объектов групповой политики (GPO). Службы Azure AD DS содержат встроенные GPO для контейнеров AADDC Users и AADDC Computers. Вы можете изменить эти встроенные GPO, чтобы настроить групповую политику под потребности своей среды. Участники группы администраторов Azure AD DC обладают правами администрирования групповых политик в домене Azure AD DS, а также могут создавать настраиваемые GPO и подразделения. Дополнительные сведения о том, что такое групповая политика и как она работает, см. в статье [Обзор групповой политики](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

В гибридной среде групповые политики, настроенные в локальной среде AD DS, не синхронизируются с Azure AD DS. Чтобы определить параметры конфигурации для пользователей или компьютеров в Azure AD DS, измените один из стандартных объектов групповой политики или создайте собственный.

В статье [Управление групповой политикой](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) описано, как установить средства управления групповыми политиками, как изменить встроенные объекты групповой политики и как создать собственные объекты групповой политики.




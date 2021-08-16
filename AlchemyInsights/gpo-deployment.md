---
title: Развертывание GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067853"
---
# <a name="gpo-deployment"></a>Развертывание GPO

Параметры для объектов пользователей и компьютеров в доменных службах Azure Active Directory (Azure AD DS) часто управляются с помощью объектов групповой политики (GPO). Службы Azure AD DS содержат встроенные GPO для контейнеров AADDC Users и AADDC Computers. Вы можете изменить эти встроенные GPO, чтобы настроить групповую политику под потребности своей среды. Участники группы администраторов Azure AD DC обладают правами администрирования групповых политик в домене Azure AD DS, а также могут создавать настраиваемые GPO и подразделения. Дополнительные сведения о групповой политике и ее работе см. в [обзоре групповой политики.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

В гибридной среде групповые политики, настроенные в локальной среде AD DS, не синхронизируются с Azure AD DS. Чтобы определить параметры конфигурации для пользователей или компьютеров в Azure AD DS, измените один из стандартных объектов групповой политики или создайте собственный.

В статье [Управление групповой политикой](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) описано, как установить средства управления групповыми политиками, как изменить встроенные объекты групповой политики и как создать собственные объекты групповой политики.

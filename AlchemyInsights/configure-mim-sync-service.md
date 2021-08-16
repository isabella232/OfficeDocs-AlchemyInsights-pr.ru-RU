---
title: Настройка службы синхронизации MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978498"
---
# <a name="configure-mim-sync-service"></a>Настройка службы синхронизации MIM

Служба синхронизации Microsoft Identity Manager (MIM) является компонентом MIM. Это централизованная локальная служба, хранящая и интегрирующая информацию для организаций с несколькими локальными каталогами и базами данных. Вы можете устранить проблему с синхронизацией MIM, если проблема была устранена в недавнем обновлении MIM или это одна из других проблем, упомянутых в разделе ниже.

**Рекомендуемые действия**

1. Используйте последнее обновление службы синхронизации MIM и проверьте [заметки о выпуске службы синхронизации MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history), чтобы узнать, устранена ли проблема в обновлении.
2. Если проблема связана с соединителем Generic LDAP, Generic SQL, Lotus Domino или Web Services, используйте последнее обновление [общих соединителей](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Если запуск синхронизации MIM останавливается из-за ошибки, просмотрите таблицу [кодов ошибок](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes), чтобы определить возможные причины.
4. Если запуск останавливается с сообщением **extension-dll-exception**, щелкните эту фразу, чтобы открыть окно **свойств объекта пространства соединителя**, и нажмите **Трассировка стека...** для получения дополнительных сведений об основной причине, как описано в разделе [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Если компонент службы уведомления об изменении паролей (PCNS) сообщает об **ошибке 6025** в журнале событий во время синхронизации паролей, см. руководство по устранению неполадок [PCNS сообщает об ошибке 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Если полная синхронизация с агентом управления службы FIM выполняется медленно, проверьте параметр **auto grow** для TempDB, как описано в статье [Устранение неполадок с медленной или зависающей полной синхронизацией](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Если вы столкнулись с ошибкой остановки сервера с сообщением failed-creation-via-web-services при использовании агента управления службы FIM, см. обзор причин в разделе [Сведения службы поддержки: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services).


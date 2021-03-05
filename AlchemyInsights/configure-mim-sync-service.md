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
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430771"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="b5aa3-102">Настройка службы синхронизации MIM</span><span class="sxs-lookup"><span data-stu-id="b5aa3-102">Configure MIM Sync service</span></span>

<span data-ttu-id="b5aa3-103">Служба синхронизации Microsoft Identity Manager (MIM) является компонентом MIM.</span><span class="sxs-lookup"><span data-stu-id="b5aa3-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="b5aa3-104">Это централизованная локальная служба, хранящая и интегрирующая информацию для организаций с несколькими локальными каталогами и базами данных.</span><span class="sxs-lookup"><span data-stu-id="b5aa3-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="b5aa3-105">Вы можете устранить проблему с синхронизацией MIM, если проблема была устранена в недавнем обновлении MIM или это одна из других проблем, упомянутых в разделе ниже.</span><span class="sxs-lookup"><span data-stu-id="b5aa3-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="b5aa3-106">**Рекомендуемые действия**</span><span class="sxs-lookup"><span data-stu-id="b5aa3-106">**Recommended steps**</span></span>

1. <span data-ttu-id="b5aa3-107">Используйте последнее обновление службы синхронизации MIM и проверьте [заметки о выпуске службы синхронизации MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history), чтобы узнать, устранена ли проблема в обновлении.</span><span class="sxs-lookup"><span data-stu-id="b5aa3-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="b5aa3-108">Если проблема связана с соединителем Generic LDAP, Generic SQL, Lotus Domino или Web Services, используйте последнее обновление [общих соединителей](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="b5aa3-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="b5aa3-109">Если запуск синхронизации MIM останавливается из-за ошибки, просмотрите таблицу [кодов ошибок](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes), чтобы определить возможные причины.</span><span class="sxs-lookup"><span data-stu-id="b5aa3-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="b5aa3-110">Если запуск останавливается с сообщением **extension-dll-exception**, щелкните эту фразу, чтобы открыть окно **свойств объекта пространства соединителя**, и нажмите **Трассировка стека...** для получения дополнительных сведений об основной причине, как описано в разделе [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="b5aa3-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="b5aa3-111">Если компонент службы уведомления об изменении паролей (PCNS) сообщает об **ошибке 6025** в журнале событий во время синхронизации паролей, см. руководство по устранению неполадок [PCNS сообщает об ошибке 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="b5aa3-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="b5aa3-112">Если полная синхронизация с агентом управления службы FIM выполняется медленно, проверьте параметр **auto grow** для TempDB, как описано в статье [Устранение неполадок с медленной или зависающей полной синхронизацией](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="b5aa3-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="b5aa3-113">Если вы столкнулись с ошибкой остановки сервера с сообщением failed-creation-via-web-services при использовании агента управления службы FIM, см. обзор причин в разделе [Сведения службы поддержки: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services).</span><span class="sxs-lookup"><span data-stu-id="b5aa3-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>


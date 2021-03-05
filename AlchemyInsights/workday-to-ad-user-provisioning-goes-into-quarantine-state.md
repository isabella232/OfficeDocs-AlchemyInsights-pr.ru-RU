---
title: Подготовка пользователей из Workday в AD переходит в состояние карантина
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430772"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="eba73-102">Подготовка пользователей из Workday в AD переходит в состояние карантина</span><span class="sxs-lookup"><span data-stu-id="eba73-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="eba73-103">**Подготовка пользователей из Workday в AD переходит в состояние карантина, и в AD не создаются пользователи**</span><span class="sxs-lookup"><span data-stu-id="eba73-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="eba73-104">Задание подготовки пользователей из Workday в AD перешло в состояние карантина, а в журналах аудита отображаются события сбоя экспорта с сообщением **Ошибка. OperationsError-SvcErr: произошла ошибка операции. Главная ссылка для службы каталогов не настроена. Таким образом, службе каталогов не удастся выдать ссылки на объекты вне этого леса**.</span><span class="sxs-lookup"><span data-stu-id="eba73-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="eba73-105">Эта ошибка обычно возникает, если неправильно задано подразделение контейнера Active Directory или имеются проблемы с сопоставлением выражения, примененным для **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="eba73-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="eba73-106">Проверьте, нет ли опечаток в подразделении по умолчанию для параметра **Новые пользователи**.</span><span class="sxs-lookup"><span data-stu-id="eba73-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="eba73-107">Убедитесь, что указанное подразделение уже существует в AD.</span><span class="sxs-lookup"><span data-stu-id="eba73-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="eba73-108">Если вы используете атрибут **parentDistinguishedName** в сопоставлении атрибутов, убедитесь, что он всегда оценивается по известному контейнеру в домене AD.</span><span class="sxs-lookup"><span data-stu-id="eba73-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="eba73-109">Проверьте событие экспорта в журналах аудита, чтобы увидеть созданное значение.</span><span class="sxs-lookup"><span data-stu-id="eba73-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="eba73-110">Дополнительные сведения о настройке Workday для автоматической подготовки см. в статье [Руководство по настройке Workday для автоматической подготовки пользователей](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="eba73-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>


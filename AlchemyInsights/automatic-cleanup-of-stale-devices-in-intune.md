---
title: Автоматическая очистка неактивных устройств в Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715034"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="2e343-102">Автоматическая очистка неактивных устройств в Intune</span><span class="sxs-lookup"><span data-stu-id="2e343-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="2e343-103">Intune позволяет администратору настраивать интервал времени 90–270 дней, по окончании которого неактивные устройства удаляются из службы.</span><span class="sxs-lookup"><span data-stu-id="2e343-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="2e343-104">Это параметр для всей организации, который вступает в силу сразу после активации.</span><span class="sxs-lookup"><span data-stu-id="2e343-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="2e343-105">Все устройства, которые не были возвращены на сервер Intune в течение периода, превышающего значение параметра, удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="2e343-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="2e343-106">**Примечание.** Для этого действия очистки доступны только объекты устройств MDM.</span><span class="sxs-lookup"><span data-stu-id="2e343-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="2e343-107">Объекты устройств только с EAS исключаются.</span><span class="sxs-lookup"><span data-stu-id="2e343-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="2e343-108">Дополнительные сведения об удалении устройства с учетом параметра очистки устройств и его состояния</span><span class="sxs-lookup"><span data-stu-id="2e343-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="2e343-109">Параметр: **Удаление устройств после даты последнего возврата: да (указано определенное значение (N) в днях)**</span><span class="sxs-lookup"><span data-stu-id="2e343-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="2e343-110">С учетом значения (N), настроенного для параметра, служба Intune удаляет устройство через указанное количество дней после последнего успешного возврата.</span><span class="sxs-lookup"><span data-stu-id="2e343-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="2e343-111">Параметр: **Удаление устройств после даты последнего возврата: нет**</span><span class="sxs-lookup"><span data-stu-id="2e343-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="2e343-112">Устройство удаляется через 180 дней после истечения срока действия его сертификата, если он не был обновлен.</span><span class="sxs-lookup"><span data-stu-id="2e343-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="2e343-113">**Примечание.** В обоих случаях устройство должно быть успешно зарегистрировано в Intune.</span><span class="sxs-lookup"><span data-stu-id="2e343-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="2e343-114">Регистрация выполняется во время первого возврата устройства в службу Intune.</span><span class="sxs-lookup"><span data-stu-id="2e343-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="2e343-115">Если устройство успешно подает заявку на регистрацию в Intune, но его не удается зарегистрировать, оно удаляется через 270 дней после подачи заявки.</span><span class="sxs-lookup"><span data-stu-id="2e343-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="2e343-116">(90 дней, чтобы пометить устройство как отозванное, и еще 180 дней, чтобы удалить запись.)</span><span class="sxs-lookup"><span data-stu-id="2e343-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="2e343-117">В настоящее время консоль Intune не включает механизм установки даты окончания срока действия сертификата для указанного устройства.</span><span class="sxs-lookup"><span data-stu-id="2e343-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>
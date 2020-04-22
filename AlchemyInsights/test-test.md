---
title: Условия, отсутствующие в банке терминов SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766866"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f4cee-102">Включение шифрования BitLocker с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="f4cee-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="f4cee-103">Политика Endpoint Protection Intune можно использовать для настройки параметров шифрования Боитлоккер для устройств с Windows, как описано в разделе: Windows10 (и более поздних версий) для защиты устройств с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="f4cee-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="f4cee-104">Следует учитывать, что многие новые устройства под управлением Windows 10 поддерживают автоматическое шифрование BitLocker, которое запускается без применения политики MDM.</span><span class="sxs-lookup"><span data-stu-id="f4cee-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f4cee-105">Это может повлиять на применение политики, если настроены параметры, не установленные по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f4cee-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="f4cee-106">Более подробную информацию можно узнать в статье вопросы и ответы.</span><span class="sxs-lookup"><span data-stu-id="f4cee-106">See FAQ for more detail.</span></span>


<span data-ttu-id="f4cee-107">Вопросы  и ответы: какие выпуски Windows поддерживают шифрование устройств с помощью политики Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="f4cee-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="f4cee-108"> О. параметры в политике Endpoint Protection в Intune реализуются с помощью поставщика службы шифрования BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f4cee-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="f4cee-109">Не все выпуски и сборки Windows поддерживают CSP BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="f4cee-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="f4cee-110">В настоящее время выпуски Windows: Enterprise; Поддерживаются образование, мобильные устройства, мобильные предприятия и профессиональный (из сборки 1809 в сторону).</span><span class="sxs-lookup"><span data-stu-id="f4cee-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="f4cee-111">В. Если устройство уже зашифровано с помощью BitLocker с использованием параметров операционной системы по умолчанию для метода шифрования и стойкости шифра (КСТС-AES-128), будет ли политика с другими параметрами автоматически вызывать повторное шифрование диска с новыми параметрами?</span><span class="sxs-lookup"><span data-stu-id="f4cee-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="f4cee-112">A: нет.</span><span class="sxs-lookup"><span data-stu-id="f4cee-112">A: No.</span></span> <span data-ttu-id="f4cee-113">Чтобы применить новые параметры шифра, необходимо сначала расшифровать диск.</span><span class="sxs-lookup"><span data-stu-id="f4cee-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="f4cee-114">Примечание для устройств, зарегистрированных с помощью автопилота. Автоматическое шифрование, которое возникает во время OOBE, не активируется, пока не будет оценена политика Intune, что позволяет использовать параметры на основе политики вместо значений по умолчанию для ОС</span><span class="sxs-lookup"><span data-stu-id="f4cee-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="f4cee-115">В. Если устройство зашифровано в результате применения политики Intune, будет ли оно расшифровано при удалении этой политики?</span><span class="sxs-lookup"><span data-stu-id="f4cee-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="f4cee-116">А: Удаление политики, связанной с шифрованием, не приводит к расшифровке настроенных дисков.</span><span class="sxs-lookup"><span data-stu-id="f4cee-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="f4cee-117">Вопрос: почему политика соответствия Intune показывает, что на устройстве нет "BitLocker Enabled", но это так?</span><span class="sxs-lookup"><span data-stu-id="f4cee-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="f4cee-118">A: параметр "BitLocker Enabled" в политике соответствия Intune использует клиент подтверждения работоспособности устройств Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="f4cee-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f4cee-119">Этот клиент измеряет состояние устройства во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="f4cee-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="f4cee-120">Таким образом, если устройство не было перезагружено с момента завершения шифрования BitLocker, клиентская служба DHA не будет сообщать о том, что BitLocker активен.</span><span class="sxs-lookup"><span data-stu-id="f4cee-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>
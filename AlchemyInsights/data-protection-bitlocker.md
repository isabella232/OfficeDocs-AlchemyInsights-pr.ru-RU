---
title: Защита с помощью BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908722"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="34cd3-102">Включение шифрования BitLocker с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="34cd3-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="34cd3-103">Политика Endpoint Protection Intune можно использовать для настройки параметров шифрования BitLocker для устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="34cd3-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="34cd3-104">Дополнительные сведения см. [в статье Windows 10 (и более поздних версий) для защиты устройств с помощью Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="34cd3-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="34cd3-105">Следует учитывать, что многие новые устройства под управлением Windows 10 поддерживают автоматическое шифрование BitLocker, которое запускается без применения политики MDM.</span><span class="sxs-lookup"><span data-stu-id="34cd3-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="34cd3-106">Это может повлиять на применение политики, если настроены параметры, не установленные по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="34cd3-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="34cd3-107">Более подробную информацию можно найти в следующих статьях часто задаваемых вопросов.</span><span class="sxs-lookup"><span data-stu-id="34cd3-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="34cd3-108">Сведения об устранении неполадок, связанных с BitLocker, приведены [в разделе Устранение неполадок в политиках BitLocker в Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="34cd3-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="34cd3-109">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="34cd3-109">**FAQ**</span></span>

 <span data-ttu-id="34cd3-110">Вопрос: какие выпуски Windows поддерживают шифрование устройств с помощью политики Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="34cd3-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="34cd3-111">О. параметры в политике Endpoint Protection в Intune реализуются с помощью [поставщика службы шифрования BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="34cd3-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="34cd3-112">Не все выпуски или сборки Windows поддерживают CSP BitLocker.</span><span class="sxs-lookup"><span data-stu-id="34cd3-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="34cd3-113">В настоящее время поддерживаются следующие выпуски Windows: Enterprise, образование, мобильный, Мобильный предприятие и профессиональный (сборка 1809 и более поздние версии).</span><span class="sxs-lookup"><span data-stu-id="34cd3-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="34cd3-114">В. Если устройство уже зашифровано с помощью BitLocker с использованием параметров по умолчанию для метода шифрования и стойкости шифра (КСТС-AES-128), будет ли политика с другими параметрами автоматически инициировать повторное шифрование диска с новыми параметрами?</span><span class="sxs-lookup"><span data-stu-id="34cd3-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="34cd3-115">A: нет.</span><span class="sxs-lookup"><span data-stu-id="34cd3-115">A: No.</span></span> <span data-ttu-id="34cd3-116">Чтобы применить новые параметры шифра, необходимо сначала расшифровать диск.</span><span class="sxs-lookup"><span data-stu-id="34cd3-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="34cd3-117">**Примечание:** Для устройств, зарегистрированных с помощью автопилота, автоматическое шифрование, которое будет происходить во время OOBE, не активируется до оценки политики Intune, что позволяет использовать параметры политики на месте значений по умолчанию для ОС.</span><span class="sxs-lookup"><span data-stu-id="34cd3-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="34cd3-118">Вопрос: Если устройство зашифровано в результате применения политики Intune, будет ли оно расшифровано при удалении этой политики?</span><span class="sxs-lookup"><span data-stu-id="34cd3-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="34cd3-119">А: Удаление политики, связанной с шифрованием, не приводит к расшифровке настроенных дисков.</span><span class="sxs-lookup"><span data-stu-id="34cd3-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="34cd3-120">Вопрос: почему политика соответствия Intune показывает, что на устройстве не включен BitLocker, даже если это так?</span><span class="sxs-lookup"><span data-stu-id="34cd3-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="34cd3-121">A: параметр "BitLocker Enabled" в политике соответствия Intune использует клиент подтверждения работоспособности устройств Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="34cd3-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="34cd3-122">Этот клиент измеряет состояние устройства во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="34cd3-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="34cd3-123">Таким образом, если устройство не было перезагружено с момента завершения шифрования BitLocker, клиентская служба DHA не будет сообщать о том, что BitLocker активен.</span><span class="sxs-lookup"><span data-stu-id="34cd3-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 
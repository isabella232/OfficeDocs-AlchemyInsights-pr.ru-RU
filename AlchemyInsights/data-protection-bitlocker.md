---
title: DataProtection — Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768830"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="157f5-102">Включение шифрования BitLocker с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="157f5-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="157f5-103">Для настройки параметров шифрования Bitlocker для устройств с Windows можно использовать политику защиты конечных точек Intune.</span><span class="sxs-lookup"><span data-stu-id="157f5-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="157f5-104">Дополнительные сведения см. в [настройках Windows 10 (и](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)более поздних) для защиты устройств с помощью Intune.</span><span class="sxs-lookup"><span data-stu-id="157f5-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="157f5-105">Следует помнить, что многие новые устройства под управлением Windows 10 поддерживают автоматическое шифрование Bitlocker, которое запускается без применения политики MDM.</span><span class="sxs-lookup"><span data-stu-id="157f5-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="157f5-106">Это может повлиять на применение политики, если настроены нестандартные параметры.</span><span class="sxs-lookup"><span data-stu-id="157f5-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="157f5-107">Дополнительные вопросы и вопросы см. в следующих подробностях.</span><span class="sxs-lookup"><span data-stu-id="157f5-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="157f5-108">Сведения об устранении неполадок bitlocker см. в сведениях об устранении неполадок политик [BitLocker в Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)</span><span class="sxs-lookup"><span data-stu-id="157f5-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="157f5-109">**Вопросы и ответы**</span><span class="sxs-lookup"><span data-stu-id="157f5-109">**FAQ**</span></span>

<span data-ttu-id="157f5-110">Вопрос. Какие выпуски Windows поддерживают шифрование устройств с помощью политики защиты конечных точек?</span><span class="sxs-lookup"><span data-stu-id="157f5-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="157f5-111">О. Параметры в политике защиты конечных точек Intune реализованы с помощью [CSP Bitlocker.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="157f5-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="157f5-112">Не все выпуски или сборки Windows поддерживают bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="157f5-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="157f5-113">Вопрос. Как включить BitLocker на устройствах без необходимости взаимодействия с пользователем?</span><span class="sxs-lookup"><span data-stu-id="157f5-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="157f5-114">О. При условии, что необходимые требования выполнены, можно включить "Тихое шифрование" Bitlocker через Intune.</span><span class="sxs-lookup"><span data-stu-id="157f5-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="157f5-115">Подробные сведения о требованиях к устройству и примеры параметров политики для обеспечения возможности шифрования в тихом режиме см. в следующем док-сообщении: автоматически включить шифрование [Bitlocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)</span><span class="sxs-lookup"><span data-stu-id="157f5-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="157f5-116">Вопрос. Если устройство уже зашифровано с помощью Bitlocker с помощью параметров ос по умолчанию для метода шифрования и уровня шифра (XTS-AES-128), будет ли применяться политика с другими настройками, автоматически инициирует повторное шифрование диска с новыми настройками?</span><span class="sxs-lookup"><span data-stu-id="157f5-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="157f5-117">Ответ. Нет.</span><span class="sxs-lookup"><span data-stu-id="157f5-117">A: No.</span></span> <span data-ttu-id="157f5-118">Чтобы применить новые параметры шифра, сначала необходимо расшифровать диск.</span><span class="sxs-lookup"><span data-stu-id="157f5-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="157f5-119">**Примечание.** Для устройств, зарегистрированных с помощью Autopilot, автоматическое шифрование, которое будет происходить во время запуска при OOBE, не запускается до тех пор, пока не будет оценена политика Intune, которая позволяет использовать параметры на основе политики, а не значения по умолчанию ОС.</span><span class="sxs-lookup"><span data-stu-id="157f5-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="157f5-120">Вопрос. Если устройство зашифровано в результате применения политики Intune, будет ли оно расшифровываться при удалении этой политики?</span><span class="sxs-lookup"><span data-stu-id="157f5-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="157f5-121">О. Удаление политики, связанной с шифрованием, НЕ приводит к расшифровке настроенных дисков.</span><span class="sxs-lookup"><span data-stu-id="157f5-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="157f5-122">Вопрос. Почему политика соответствия требованиям Intune показывает, что на моем устройстве не включен Bitlocker, хотя это так?</span><span class="sxs-lookup"><span data-stu-id="157f5-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="157f5-123">О. Параметр "Bitlocker enabled" в политике соответствия требованиям Intune использует клиент службы DHA.</span><span class="sxs-lookup"><span data-stu-id="157f5-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="157f5-124">Этот клиент измеряет только состояние устройства во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="157f5-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="157f5-125">Поэтому если устройство не было перезагружается с момента завершения шифрования Bitlocker, клиентская служба DHA не будет сообщать о bitlocker как активном.</span><span class="sxs-lookup"><span data-stu-id="157f5-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 
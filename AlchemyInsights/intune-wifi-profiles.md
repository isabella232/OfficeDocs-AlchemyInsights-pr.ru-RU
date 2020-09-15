---
title: Профили Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696274"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="6b508-102">Профили Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="6b508-103">Успешное подключение Wi-Fi для клиентов MDM зависит от правильно развернутого профиля, который отражает требования корпоративной инфраструктуры Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6b508-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="6b508-104">Просмотреть соответствующие настройки для клиентских платформ, которые вы изучаете, можно в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="6b508-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="6b508-105">Добавление параметров Wi-Fi для устройств с Android в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="6b508-106">Добавление параметров Wi-Fi для выделенных и полностью управляемых устройств с Android Enterprise в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="6b508-107">Добавление параметров Wi-Fi для устройств iOS и iPadOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="6b508-108">Добавление параметров Wi-Fi для устройств с Windows 10 и более поздних версий в Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="6b508-109">Добавление параметров Wi-Fi для устройств Windows в Intune</span><span class="sxs-lookup"><span data-stu-id="6b508-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="6b508-110">**Распространенные проблемы**</span><span class="sxs-lookup"><span data-stu-id="6b508-110">**Common Issues**</span></span>

<span data-ttu-id="6b508-111">**Я выполняю развертывание профиля Wi-Fi, который зависит от развернутого сертификата, указанного в профиле Wi-Fi. Однако в профилях конфигурации отображается состояние ошибки.**</span><span class="sxs-lookup"><span data-stu-id="6b508-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="6b508-112">Убедитесь, что устройство получило сертификат.</span><span class="sxs-lookup"><span data-stu-id="6b508-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="6b508-113">В Intune перейдите в раздел **Все устройства** и выберите устройство > **Конфигурация устройства**.</span><span class="sxs-lookup"><span data-stu-id="6b508-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="6b508-114">Убедитесь, что все ожидаемые профили указаны и в успешном состоянии.</span><span class="sxs-lookup"><span data-stu-id="6b508-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="6b508-115">При наличии промежуточных сертификатов в цепочке сертификатов для профиля Android убедитесь, что они развернуты на устройствах с Android.</span><span class="sxs-lookup"><span data-stu-id="6b508-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="6b508-116">Чтобы проверить состояние сертификата, перейдите в раздел **Конфигурация устройств** > **Профили** > **Промежуточный центр сертификации Android** > **Свойства** > **Доверенный сертификат**.</span><span class="sxs-lookup"><span data-stu-id="6b508-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="6b508-117">Если по-прежнему будут возникать ошибки, см. разделы "Процедуры" и "Устранение неполадок".</span><span class="sxs-lookup"><span data-stu-id="6b508-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="6b508-118">Дополнительные сведения см. в статье [Общие сведения об устранении неполадок профилей сертификатов SCEP в Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6b508-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="6b508-119">**Выполнено развертывание профиля Wi-Fi на устройстве. Intune показывает, что все прошло успешно, но устройство не подключается к Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="6b508-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="6b508-120">Статус «успешно» означает, что приложение Intune успешно развернуло профиль в настроенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="6b508-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="6b508-121">Однако эти конфигурации могут не соответствовать требованиям вашей сети и (или) проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6b508-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="6b508-122">Дополнительные сведения о попытках подключения см. в журналах службы инфраструктуры и проверки подлинности (на контроллере точек доступа Wi-Fi и сервере NPS/RADIUS).</span><span class="sxs-lookup"><span data-stu-id="6b508-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="6b508-123">Чтобы собрать и просмотреть журналы, вам, возможно, придется обратиться к вашей группе сетевой инфраструктуры или стороннему поставщику Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6b508-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>
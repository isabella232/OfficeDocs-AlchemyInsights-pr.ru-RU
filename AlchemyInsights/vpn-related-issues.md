---
title: Неполадки, связанные с VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726104"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="38a8a-102">Неполадки, связанные с VPN</span><span class="sxs-lookup"><span data-stu-id="38a8a-102">VPN related issues</span></span>

<span data-ttu-id="38a8a-103">Успешное подключение VPN для клиентов MDM зависит от развернутого профиля, который правильно отражает требования инфраструктуры VPN.</span><span class="sxs-lookup"><span data-stu-id="38a8a-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="38a8a-104">Соответствующие настройки для клиентских платформ, которые вы изучаете, см. в разделе:</span><span class="sxs-lookup"><span data-stu-id="38a8a-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="38a8a-105">Настройки устройств с Windows 10 и Windows Holographic для добавления VPN-соединений с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="38a8a-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="38a8a-106"> Добавить настройки VPN на устройствах iOS и iPadOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="38a8a-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="38a8a-107">Параметры устройств с Android для настройки VPN в Intune</span><span class="sxs-lookup"><span data-stu-id="38a8a-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="38a8a-108"> Добавить настройки VPN на устройствах macOS в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="38a8a-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="38a8a-109">Если ваш профиль VPN использует проверку подлинности на основе сертификатов, убедитесь, что профили корневого сертификата и проверки подлинности клиента, связанные с профилем VPN, успешно развернуты.</span><span class="sxs-lookup"><span data-stu-id="38a8a-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="38a8a-110">**Распространенные проблемы**</span><span class="sxs-lookup"><span data-stu-id="38a8a-110">**Common Issues**</span></span>

<span data-ttu-id="38a8a-111">**Я развернул профиль VPN на устройство. Intune показывает, что все прошло успешно, но устройство не подключается к VPN.**</span><span class="sxs-lookup"><span data-stu-id="38a8a-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="38a8a-112">Статус «успешно» означает, что приложение Intune успешно развернуло профиль в настроенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="38a8a-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="38a8a-113">Однако эти конфигурации могут не соответствовать требованиям вашей сети и (или) проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="38a8a-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="38a8a-114">Дополнительные сведения о попытках подключения см. в журналах службы инфраструктуры и проверки подлинности (на VPN-сервере и сервере NPS/RADIUS).</span><span class="sxs-lookup"><span data-stu-id="38a8a-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="38a8a-115">Чтобы собрать и просмотреть журналы, вам, возможно, придется обратиться к вашей группе сетевой инфраструктуры или стороннему поставщику VPN.</span><span class="sxs-lookup"><span data-stu-id="38a8a-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="38a8a-116">**При настройке пользовательской сети VPN для iOS функция VPN не становится доступной для каждого приложения.**</span><span class="sxs-lookup"><span data-stu-id="38a8a-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="38a8a-117">VPN для каждого приложения для устройств iOS в Intune в настоящий момент доступна определенному списку поставщиков и партнеров, которые также должны соответствовать предварительным требованиям к сертификату перед настройкой VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="38a8a-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="38a8a-118">Для получения более подробной информации см. раздел [Настройке виртуальной частной (VPN) сети для каждого приложения для устройств с iOS/iPadOS в Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="38a8a-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="38a8a-119">Для получения дополнительной информации обо всех типах VPN соединений в Intune, см. раздел[Создание VPN профилей для подключения к VPN серверам в Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="38a8a-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="38a8a-120">**VPN по запросу iOS не активируется, когда к настроенному домену есть доступ**</span><span class="sxs-lookup"><span data-stu-id="38a8a-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="38a8a-121">Для проверки автоматических настроек VPN установите следующие значения:</span><span class="sxs-lookup"><span data-stu-id="38a8a-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="38a8a-122">Я хочу сделать следующее: **Оценить каждую попытку подключения**</span><span class="sxs-lookup"><span data-stu-id="38a8a-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="38a8a-123">Выберите, нужно ли подключаться: **Подключить при необходимости**</span><span class="sxs-lookup"><span data-stu-id="38a8a-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="38a8a-124">Когда пользователи получают доступ к этим доменам: **имя** *целевого домена*</span><span class="sxs-lookup"><span data-stu-id="38a8a-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="38a8a-125">Если описанная выше конфигурация не была удачной, добавьте следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="38a8a-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="38a8a-126">Если этот URL-адрес недоступен, принудительно подключите VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="38a8a-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>
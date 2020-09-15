---
title: 'Устранение неполадок при развертывании сертификата проверки подлинности клиента '
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658999"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="63255-102">Устранение неполадок при развертывании сертификата проверки подлинности клиента </span><span class="sxs-lookup"><span data-stu-id="63255-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="63255-103">Сертификаты Intune NDES/SCEP и PKCS/PFX часто используются в сочетании с другими типами профилей, такими как WiFi, VPN и электронная почта, чтобы разрешить пользователям проходить проверку подлинности на корпоративных ресурсах.</span><span class="sxs-lookup"><span data-stu-id="63255-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="63255-104">Когда эти типы профиля связаны с профилем сертификата клиента, они зависят от успешности развертывания этого профиля.</span><span class="sxs-lookup"><span data-stu-id="63255-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="63255-105">Исходная настройка инфраструктуры и связанная с ней конфигурация профиля сертификата клиента часто требуют устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="63255-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="63255-106">Пошаговые инструкции по успешной настройке соединителя NDES и рекомендации по устранению неполадок для изоляции проблем с развертыванием сертификатов см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="63255-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="63255-107">Настройка инфраструктуры для поддержки SCEP с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="63255-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="63255-108">Общие сведения об устранении неполадок профилей сертификатов SCEP с помощью Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="63255-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="63255-109">Чтобы проверить конфигурацию, используйте указанные сценарии PowerShell.</span><span class="sxs-lookup"><span data-stu-id="63255-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="63255-110">Для получения дополнительных сведений см. статью [Сценарии подтверждения соединителя сертификатов Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="63255-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="63255-111">**Другие распространенные проблемы**</span><span class="sxs-lookup"><span data-stu-id="63255-111">**Other common issues**</span></span>

<span data-ttu-id="63255-112">**При попытке установить соединитель сертификатов Intune на сервере соединителя NDES выводится сообщение: "Не удается проверить пароль в запросе сертификата. Возможно, он уже использовался. Получите новый пароль для отправки с этим запросом".**</span><span class="sxs-lookup"><span data-stu-id="63255-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="63255-113">Это сообщение означает, что необходимо запустить установку соединителя сертификатов в качестве администратора.</span><span class="sxs-lookup"><span data-stu-id="63255-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="63255-114">В некоторых средах серверы, на которых запускается сертификат Intune, должны использовать прокси-сервер для подключения к Intune, поэтому и соединитель сертификатов должен использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="63255-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="63255-115">В некоторых случаях соединитель NDES игнорирует настроенные параметры прокси-сервера и может потребоваться настроить параметры прокси-сервера при запуске в контексте безопасности локальной системы.</span><span class="sxs-lookup"><span data-stu-id="63255-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="63255-116">Чтобы решить эту проблему, запустите Internet Explorer как систему и настройте прокси в IE.</span><span class="sxs-lookup"><span data-stu-id="63255-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="63255-117">После перезапуска службы соединителя Intune соединитель NDES соединяется с Intune.</span><span class="sxs-lookup"><span data-stu-id="63255-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="63255-118">**Устройства пользователей больше не получают сертификаты SCEP от NDES.**</span><span class="sxs-lookup"><span data-stu-id="63255-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="63255-119">Возможно, сертификат проверки подлинности клиента, выданный серверу NDES и указанного при установке соединителя NDES, отсутствует либо у него истек срок действия.</span><span class="sxs-lookup"><span data-stu-id="63255-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="63255-120">Для устранения проблемы:</span><span class="sxs-lookup"><span data-stu-id="63255-120">To resolve:</span></span> 
 
1. <span data-ttu-id="63255-121">Удалите соединитель NDES.</span><span class="sxs-lookup"><span data-stu-id="63255-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="63255-122">Для запроса нового сертификата проверки подлинности клиента или сертификата проверки подлинности сервера используйте указанные ниже данные:</span><span class="sxs-lookup"><span data-stu-id="63255-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="63255-123">Имя субъекта: CN=внешнее полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="63255-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="63255-124">Альтернативное имя субъекта (оба параметра обязательны): DNS=внешнее полное доменное имя, DNS=внутреннее полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="63255-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="63255-125">Переустановите соединитель NDES с новым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="63255-125">Reinstall the NDES connector with the new certificate.</span></span>
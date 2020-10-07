---
title: Развертывание приложений Win32 с помощью Intune
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
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366528"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="f768a-102">Развертывание приложений Win32 с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="f768a-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="f768a-103">Microsoft Intune дает возможность развертывать приложения Win32, включая MSI и EXE, на устройствах с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f768a-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="f768a-104">Для механизма развертывания требуется, чтобы на целевом устройстве было расширение управления Intune (IME).</span><span class="sxs-lookup"><span data-stu-id="f768a-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="f768a-105">Расширение IME устанавливается автоматически, если нацелить сценарий PowerShell или развертывание приложения Win32 на определенного пользователя или устройство.</span><span class="sxs-lookup"><span data-stu-id="f768a-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="f768a-106">Для развертывания приложений Win32 также необходимо выполнить ряд предварительных требований:</span><span class="sxs-lookup"><span data-stu-id="f768a-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="f768a-107">Поддерживаемые платформы: Windows 10 версии 1607 или более поздней (Корпоративная, Pro и для образовательных учреждений).</span><span class="sxs-lookup"><span data-stu-id="f768a-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="f768a-108">Поддерживаемые архитектуры: x86 и x64.</span><span class="sxs-lookup"><span data-stu-id="f768a-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="f768a-109">Управление устройствами: требуется присоединение к AAD и автоматическая регистрация (включая присоединение к гибридному домену и автоматическая регистрация с помощью групповой политики).</span><span class="sxs-lookup"><span data-stu-id="f768a-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="f768a-110">Формат пакета приложения: файл с расширением.**intunewin**, подготовленный с помощью [средства подготовки содержимого Win32 (Майкрософт)](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="f768a-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="f768a-111">Ограничения:</span><span class="sxs-lookup"><span data-stu-id="f768a-111">Limitations:</span></span>
    - <span data-ttu-id="f768a-112">Максимальный размер: 8 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f768a-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="f768a-113">Неподдерживаемая архитектура: ARM.</span><span class="sxs-lookup"><span data-stu-id="f768a-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="f768a-114">Прочтите документ "[Добавление, назначение и мониторинг приложений Win32 в Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" для получения сведений, связанных с этими действиями.</span><span class="sxs-lookup"><span data-stu-id="f768a-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="f768a-115">Сведения об устранении неполадок при развертывании приложений в Windows, включая приложения Win32, см. в следующих документах:</span><span class="sxs-lookup"><span data-stu-id="f768a-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="f768a-116">Устранение неполадок при установке приложений</span><span class="sxs-lookup"><span data-stu-id="f768a-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="f768a-117">Устранение неполадок приложений Win32</span><span class="sxs-lookup"><span data-stu-id="f768a-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)
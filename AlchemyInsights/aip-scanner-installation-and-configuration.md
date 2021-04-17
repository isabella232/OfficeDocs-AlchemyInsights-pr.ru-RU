---
title: 'Сканер AIP: Установка и настройка'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821676"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="9e0f6-102">Сканер AIP: Установка и настройка</span><span class="sxs-lookup"><span data-stu-id="9e0f6-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="9e0f6-103">**Чтобы установить сканер AIP, следуйте рекомендациям**:</span><span class="sxs-lookup"><span data-stu-id="9e0f6-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="9e0f6-104">Если вы выполняете обновление и не выполняете чистую установку, убедитесь в том, что вы следовали рекомендациям по [обновлению сканера Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) и для клиента унифицированных меток, см. раздел[обновление сканера Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="9e0f6-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="9e0f6-105">Убедитесь в том, что все [требования к брандмауэрам и параметрам сетевой инфраструктуры](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure) соблюдены.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="9e0f6-106">Убедитесь в том, что ваши [политики настроены](https://docs.microsoft.com/azure/information-protection/configure-policy) на автоматическое применение меток или в политике есть метка по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="9e0f6-107">Убедитесь в том, что соответствующий тип файла настроен на маркировку/защиту, как описано в разделе [Типы файлов, поддерживаемые клиентом Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="9e0f6-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="9e0f6-108">Кроме того, если вы хотите изменить стандартные параметры, следуйте следующим рекомендациям: [Изменения уровня защиты файлов по умолчанию](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="9e0f6-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="9e0f6-109">Убедитесь, что учетная запись пользователя, в которой запущена служба сканера, имеет разрешения на доступ ко всем настроенным репозиториям.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="9e0f6-110">Если проблема не устранена, экспортируйте журналы сканера и добавьте их в свой запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="9e0f6-111">**Экспорт журналов сканера Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="9e0f6-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="9e0f6-112">Перейдите в %localappdata%\Microsoft\MSIP в пользовательском контексте, в котором запущен служба сканера.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="9e0f6-113">Заархивируйте все содержимое в папку MSIP.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="9e0f6-114">Сохраните журналы в выбранном расположении и вложите их в запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="9e0f6-115">Также можно использовать [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="9e0f6-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="9e0f6-116">**Дополнительные сведения см. в разделах**:</span><span class="sxs-lookup"><span data-stu-id="9e0f6-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="9e0f6-117">Развертывание сканера Azure Information Protection для автоматической классификации и защиты файлов</span><span class="sxs-lookup"><span data-stu-id="9e0f6-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="9e0f6-118">Указание и использование параметра токена для Set-AIPAuthentication.</span><span class="sxs-lookup"><span data-stu-id="9e0f6-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="9e0f6-119">Запуск цикла обнаружения и просмотр отчетов для сканера</span><span class="sxs-lookup"><span data-stu-id="9e0f6-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="9e0f6-120">Обзор документации Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9e0f6-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- <span data-ttu-id="9e0f6-121">[Требования для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="9e0f6-121">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>
- [<span data-ttu-id="9e0f6-122">Скачать клиента Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9e0f6-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)

---
title: 'Сканер AIP: Установка и настройка'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686655"
---
# <a name="aip-scanner-installation-and-configuration"></a>Сканер AIP: Установка и настройка

**Чтобы установить сканер AIP, следуйте рекомендациям**:

1. Если вы выполняете обновление и не выполняете чистую установку, убедитесь в том, что вы следовали рекомендациям по [обновлению сканера Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) и для клиента унифицированных меток, см. раздел[обновление сканера Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Убедитесь в том, что все [требования к брандмауэрам и параметрам сетевой инфраструктуры](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure) соблюдены.
3. Убедитесь в том, что ваши [политики настроены](https://docs.microsoft.com/azure/information-protection/configure-policy) на автоматическое применение меток или в политике есть метка по умолчанию.
4. Убедитесь в том, что соответствующий тип файла настроен на маркировку/защиту, как описано в разделе [Типы файлов, поддерживаемые клиентом Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Кроме того, если вы хотите изменить стандартные параметры, следуйте следующим рекомендациям: [Изменения уровня защиты файлов по умолчанию](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Убедитесь, что учетная запись пользователя, в которой запущена служба сканера, имеет разрешения на доступ ко всем настроенным репозиториям.
6. Если проблема не устранена, экспортируйте журналы сканера и добавьте их в свой запрос в службу поддержки.

**Экспорт журналов сканера Azure Information Protection**

1. Перейдите в %localappdata%\Microsoft\MSIP в пользовательском контексте, в котором запущен служба сканера.
2. Заархивируйте все содержимое в папку MSIP.
3. Сохраните журналы в выбранном расположении и вложите их в запрос в службу поддержки.
4. Также можно использовать [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Дополнительные сведения см. в разделах**:
- [Развертывание сканера Azure Information Protection для автоматической классификации и защиты файлов](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Указание и использование параметра токена для Set-AIPAuthentication.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Запуск цикла обнаружения и просмотр отчетов для сканера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Обзор документации Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Требования для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Скачать клиента Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)

---
title: Не удается активировать Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 875026fe11d3745b587131cf0dd40a28fa005dc5
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580166"
---
# <a name="unable-to-activate-office"></a>Не удается активировать Office

- Проверьте, не истек ли срок действия вашей подписки.
- Убедитесь в наличии подписки, поддерживающей клиентские лицензии, например Office 365 бизнес или бизнес премиум, и [убедитесь, что пользователю назначена лицензия](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Убедитесь, что пользователь входит в Office с учетной записью, которой назначена лицензия.
- Проверьте [страницу работоспособности службы Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) на наличие известных проблем в службе.
- Проверьте параметры брандмауэра, антивирусной программы и прокси-сервера, чтобы убедиться, что они не блокируют доступ приложений Microsoft 365 к Интернету. См. статью [URL-адреса и диапазоны IP-адресов Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-адреса и диапазоны IP-адресов Office 365").

Воспользуйтесь следующими инструкциями по устранению неполадок:

- Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей. [Удалите](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [заново назначьте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лицензию на Office, а затем [войти в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью затронутой учетной записи пользователя.
- Запустите [средство устранения неполадок активации](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Сбросьте состояние активации Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Сбросьте состояние активации Office")
- [Запустите восстановление Office по сети](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Дополнительные решения по устранению неполадок см. в следующих статьях:  

- [Ошибки, связанные с нелицензированным продуктом и активацией Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
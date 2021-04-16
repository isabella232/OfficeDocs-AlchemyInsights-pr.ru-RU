---
title: Не удается активировать Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812585"
---
# <a name="unable-to-activate-office"></a>Не удается активировать Office

- Проверьте, не истек ли срок действия вашей подписки.
- Убедитесь в наличии подписки, поддерживающей клиентские лицензии, например Office 365 бизнес или бизнес премиум, и [убедитесь, что пользователю назначена лицензия](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Убедитесь, что пользователь входит в Office с учетной записью, которой назначена лицензия.
- Проверьте [страницу работоспособности службы Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) на наличие известных проблем в службе.
- Проверьте параметры брандмауэра, антивирусной программы и прокси-сервера, чтобы убедиться, что они не блокируют доступ приложений Microsoft 365 к Интернету. См. статью [URL-адреса и диапазоны IP-адресов Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-адреса и диапазоны IP-адресов Office 365").

**Совет**: на компьютерах с Windows можно диагностировать и автоматически устранять некоторые распространенные проблемы с входом в Office. Для использования нашего автоматического инструмента скачайте и запустите **[Помощник по поддержке и восстановлению Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)**.

Воспользуйтесь следующими инструкциями по устранению неполадок:

- Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей. [Удалите](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [заново назначьте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лицензию на Office, а затем [войти в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощью затронутой учетной записи пользователя.
- Запустите [средство устранения неполадок активации](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Сбросьте состояние активации Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Сбросьте состояние активации Office")
- [Запустите восстановление Office по сети](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Дополнительные решения по устранению неполадок см. в следующих статьях:  

- [Ошибки, связанные с нелицензированным продуктом и активацией Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
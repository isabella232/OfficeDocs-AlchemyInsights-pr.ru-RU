---
title: Устранение ошибок нелицензированных продуктов
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737966"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Предложения по устранению ошибок "нелицензированный продукт"

Чтобы устранить ошибки, связанные с "нелицензированным продуктом", выполните указанные ниже действия.

- Проверьте, не просрочено ли состояние подписки.
- Убедитесь, что у вас есть подписка на клиентские лицензии, такие как Microsoft 365 Apps для бизнеса или бизнес премиум, и [Убедитесь, что у пользователя есть назначенная лицензия](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Убедитесь, что пользователь вошел в Office с той же учетной записью, которой назначена лицензия.
- Проверьте [страницу работоспособности службы](https://docs.microsoft.com/office365/enterprise/view-service-health) , чтобы проверить наличие известных проблем со службой.
- Проверьте брандмауэр, антивирусное программное обеспечение и параметры прокси-сервера, чтобы убедиться, что они не блокируют доступ приложений Microsoft 365 к Интернету. Просмотр [URL-адресов и диапазонов IP-адресов](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Вы также можете попробовать выполнить следующие действия по устранению неполадок: 

- Откройте приложение Office и [выйдите](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) из существующих учетных записей пользователей. [Удалите](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [повторно назначьте](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лицензию Office, а затем войдите в [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) , используя затронутую учетную запись пользователя.
- Запустите [средство устранения неполадок активации](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Сбросьте состояние активации Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Выполните оперативное восстановление Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Дополнительные решения по устранению неполадок см. в следующих статьях: 

- [Ошибки, связанные с нелицензированным продуктом и активацией Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
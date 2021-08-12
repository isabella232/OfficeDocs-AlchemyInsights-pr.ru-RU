---
title: Устранение ошибок без лицензии на продукт
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957113"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Рекомендации по устранению ошибок "Нелицензирования продукта"

Чтобы устранить ошибки в "нелицензивном продукте", попробуйте следующее:

- Проверьте, истек ли срок действия подписки.
- Убедитесь, что у вас есть подписка, которая позволяет клиентские лицензии, такие как Приложения Microsoft 365 для бизнеса или бизнес-Premium, и убедитесь, что пользователю назначена [лицензия.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Убедитесь, что пользователь подписывает Office с той же учетной записью, которая имеет назначенную лицензию.
- Проверьте [страницу здоровья службы,](https://docs.microsoft.com/office365/enterprise/view-service-health) чтобы узнать, существуют ли какие-либо известные проблемы со службой.
- Проверьте параметры брандмауэра, антивирусного программного обеспечения и прокси-серверов, чтобы подтвердить, что они не Microsoft 365 приложениям доступ к Интернету. См. [url-адреса и диапазоны IP-адресов.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

Также можно попробовать следующие действия по устранению неполадок: 

- Откройте Приложение Office и [запишите все](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) существующие учетные записи пользователей. [Удалите](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [и переназначите](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office лицензию, а затем вопишите Office [с](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) помощью учетной записи пострадавшего пользователя.
- Запустите [устранение неполадок активации.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Сбросьте состояние активации Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Выполните онлайн-ремонт Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Дополнительные решения по устранению неполадок см. в следующих статьях: 

- [Ошибки, связанные с нелицензированным продуктом и активацией Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Ошибка "Не удается подключиться к вашей учетной записи. Повторите попытку позже" при активации Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
---
title: Не работает переописка пароля
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232784"
---
# <a name="password-writeback-is-not-working"></a>Не работает переописка пароля

**У меня возникают проблемы с настройкой перео записи паролей**

- Функция записи паролей является важной функцией.
- Убедитесь, что вы понимаете требования к лицензированию:
  - В вашей организации должна быть хотя бы одна лицензия
  - **Только облачные пользователи** : любой платный SKU Office 365 (O365) или Azure AD Basic
  - **Облачные и/или** локально пользователи — Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)
    - Дополнительные информацию о требованиях к лицензированию см. в подраздиниях о требованиях лицензирования для самостоятельного сброса [паролей Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- У вас есть хотя бы одна учетная запись администратора и одна тестовая учетная запись пользователя с одной из соответствующих лицензий.
- Для работы с записью пароля необходимо подключить Azure AD Connect к эмулятору основного контроллера домена. Вы можете настроить Azure AD Connect для использования основного  контроллера домена, щелкнув правой кнопкой мыши свойства соединителя синхронизации Active Directory и выбрав разделы **каталогов.** После этого найди **раздел** параметров подключения контроллера домена и поимейте, что в поле с заголовком "Использовать только предпочтительные **контроллеры домена".**
  > [!NOTE]
  > Если предпочтительный dc не является эмулятором PDC, Azure AD Connect по-прежнему будет связываться с PDC для записи пароля.
- Сброс пароля настроен и включен в клиенте. Дополнительные сведения см. в подстановлении пользователями [паролей Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Убедитесь, что учетная запись администратора, используемая для обеспечения записи пароля, является учетной записью администратора облака (созданная в Azure AD, а не локальной службе AD)
- У вас есть локальное развертывание AD с одним или несколькими лесами под управлением Windows Server 2008 R2, Windows Server 2012 или Windows Server 2012 R2 с последними пакетами обновления
- У вас установлено средство Azure AD Connect и вы подготовили среду AD для синхронизации с облаком. Перед тестированием записи пароля убедитесь, что сначала вы выполните полный импорт и полную синхронизацию из AD и Azure AD в Azure AD Connect.
- Дополнительные узнать, как сделать полную синхронизацию [и полный импорт в Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**У меня возникла проблема с подключением для записи паролей**

1. Скачивание и включении последней версии [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Конфигурация брандмауэра: средству Azure AD Connect (1.1.443 и выше) потребуется исходящие **HTTPS-доступ** к:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Разрешить простаивающим подключениям сохраняться не менее 2-3 минут

**У меня по-прежнему возникают проблемы с переописаемой паролем**

- Если у вас по-прежнему возникли трудности, попробуйте отключить и повторно включив службу записи паролей в средстве Azure AD Connect
- Чтобы узнать больше, узнайте, как отключить и повторно включить возможность записи [паролей](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)

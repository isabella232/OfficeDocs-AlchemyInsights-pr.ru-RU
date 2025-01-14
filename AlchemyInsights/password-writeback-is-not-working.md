---
title: Возвращение пароля не работает
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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324936"
---
# <a name="password-writeback-is-not-working"></a>Возвращение пароля не работает

**У меня возникают проблемы с настройкой записи пароля**

- Возвращение пароля — это функция премиум-класса.
- Убедитесь, что вы понимаете требования к лицензированию:
  - В организации должна быть назначена по крайней мере одна лицензия
  - **Только пользователи облака** — Office 365 (O365) платные SKU или Azure AD Basic
  - **Облачные и/или** локально пользователи — Azure AD Premium P1 или P2, Enterprise Mobility + Security (EMS) или Secure Productive Enterprise (SPE)
    - Дополнительные новости о требованиях к лицензированию см. в см. в руб. Требования к лицензированию для сброса пароля [самообслуживающихся Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- У вас есть по крайней мере одна учетная запись администратора и одна тестовая учетная запись пользователя с соответствующей лицензией.
- Необходимо подключить Azure AD Подключение к контроллеру первичного домена Emulator для списания пароля для работы. Вы можете настроить Azure AD Подключение для использования контроллера первичного  домена, щелкнув правой кнопкой мыши по свойствам соединиттеля синхронизации Active Directory, а затем выбрав разделы настройки каталогов.  Оттуда и обратитесь к разделу **параметры** параметров подключения контроллера домена и проверьте поле под названием использовать только **предпочтительные контроллеры домена**.
    **Примечание.** Если предпочтительный DC не является эмулятором PDC, Azure AD Подключение по-прежнему будет работать с PDC для списания паролей.
- Сброс пароля был настроен и включен в клиенте. Дополнительные сведения см. в [дополнительных сведениях, которые позволяют пользователям сбросить пароли Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Убедитесь, что учетная запись администратора, используемая для списания пароля, является учетной записью облачного администратора (созданная в Azure AD не локальной AD)
- Локальное развертывание AD с одним или несколькими лесами работает Windows Server 2008 R2, Windows Server 2012 или Windows Server 2012 R2 с установленными последними пакетами служб
- Установлено средство Azure AD Подключение и подготовлена среда AD для синхронизации с облаком. Перед тестированием записи пароля убедитесь, что сначала выполните полный импорт и полную синхронизацию с AD и Azure AD в Azure AD Подключение.
- Дополнительные дополнительные информации см. в том, как полностью синхронизировать и полностью импортировать в [Azure AD Подключение](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**У меня возникли проблемы с подключением к записи паролей**

1. Скачайте и вдайте последнюю версию [Azure AD Подключение](https://www.microsoft.com/download/details.aspx?id=47594)
2. Конфигурация брандмауэра: инструменту Azure AD Подключение (1.1.443 и выше) потребуется исходящие **https-доступ** к:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Разрешить неработающим подключениям сохраняться не менее 2-3 минут

**У меня по-прежнему возникают проблемы с возвращением пароля**

- Если у вас по-прежнему возникли проблемы, попробуйте отключить и повторно включив службу записи паролей в инструменте Azure AD Подключение.
- Дополнительные возможности см. в дополнительных подробной информации об отключении и [повторном включаемом списывке паролей](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)

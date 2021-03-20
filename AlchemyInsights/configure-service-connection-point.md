---
title: Настройка точки подключения службы (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898066"
---
# <a name="configure-service-connection-point-scp"></a>Настройка точки подключения службы (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Причина**: не удается прочитать объект SCP и получить сведения о клиенте Azure AD
- **Решение**: обратитесь к разделу [Настройка точки подключения службы](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**План действий**

- Проверьте, получен ли устройством объект групповой политики (GPO) для контролируемой проверки.
- Убедитесь, что GPO создал ключи реестра.
- Убедитесь, что у вас есть 2 ключа, созданных с помощью вашего ИД каталога и домена onmicrosoft.

**Настройка параметра реестра на стороне клиента для SCP**

Используйте следующий пример для создания объекта групповой политики (GPO) для развертывания параметра реестра, который настраивает запись SCP в реестре ваших устройств.

1. Откройте консоль управления групповыми политиками и создайте новый GPO в вашем домене.
     - Дайте новому GPO имя (например, ClientSideSCP)

2. Отредактируйте GPO и найдите следующий путь: **Конфигурация компьютера > Параметры > Параметры Windows > Реестр**.

3. Щелкните правой кнопкой мыши **Реестр** и выберите **Создать > Элемент реестра**.

4. На вкладке **Общие** настройте следующие параметры:
  
- **Действие**: обновление
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Путь к разделу**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Имя значения**: TenantId
    
- Тип значения: **REG_SZ**
    
- **Значение**: GUID или ИД каталога экземпляра Azure AD (это значение можно найти на портале **Azure > Azure Active Directory > Свойства > ИД каталога**)
 
- Нажмите кнопку **ОК**.
 
5. Щелкните правой кнопкой мыши **Реестр** и выберите **Создать > Элемент реестра**.

6. На вкладке **Общие** настройте следующие параметры:
  
- **Действие**: обновление
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Путь к разделу**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Имя значения**: TenantName
    
- Тип значения: **REG_SZ**
    
- **Значение**: ваше проверенное доменное имя, если вы используете интегрированную среду, например AD FS. Проверенное доменное имя или onmicrosoft.com доменное имя (например, contoso.onmicrosoft).com, если вы используете управлевую среду

- Нажмите кнопку **ОК**.

7. Закройте редактор только что созданного GPO.

8. Привяжите только что созданный GPO к нужному OU, содержащему компьютеры, объединенные доменом и принадлежащие к вашей группе контролируемого развертывания.

Дополнительные сведения см. в статьях [Управляемая проверка гибридного соединения Azure AD — Azure AD |  Документация Майкрософт](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) и [Устранение неполадок с гибридными устройствами, подключенными к Azure Active Directory| Документация Майкрософт](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).










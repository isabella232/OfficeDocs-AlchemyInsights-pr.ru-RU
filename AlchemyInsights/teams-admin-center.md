---
title: Центр администрирования Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670377"
---
# <a name="teams-admin-center"></a>Центр администрирования Teams

Ознакомьтесь с управлением Teams с помощью [Центра администрирования Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Если вам не удается получить доступ к Центру администрирования Teams, проверьте следующее:

- Проверьте, что вы разрешили соответствующие [IP-адреса и URL-адреса Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всех устройствах периметра (в брандмауэре и т. д.) и в правилах брандмауэра на локальном компьютере.
- Убедитесь, что данные входа, используемые для доступа к порталу администрирования Teams, соответствуют имени пользователя, указанному на [портале администрирования Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Если пользователи не отображаются в Центре администрирования Teams, проверьте следующее:

- Вы создали пользователей или назначили лицензии в течение последних 24 часов? Подождите не менее 24 часов, прежде чем создавать запрос в службу поддержки.
- Убедитесь, что вам назначены соответствующие лицензии.
- Если вы пользуетесь локальной службой Active Directory, убедитесь в том, что [значение msRTCSIP-PrimaryUserAddress или адреса SIP в поле ProxyAddresses в локальной службе Active Directory уникально и его формат соответствует ](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** пользователя в [Центре администрирования Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Если вы планируете использовать развертывание Skype для бизнеса Server и разместить пользователей как локально, так и в сети, следуйте инструкциям в разделе **"Настройка гибридной среды для Teams и Skype для бизнеса в Интернете"** на информационной панели Skype for Business Server и переместите пользователей в Интернет.

---
title: Профили Wi-Fi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028233"
---
# <a name="intune-wi-fi-profiles"></a>Профили Wi-Fi Intune

Успешное подключение Wi-Fi для клиентов MDM зависит от правильно развернутого профиля, который отражает требования корпоративной инфраструктуры Wi-Fi. Просмотреть соответствующие настройки для клиентских платформ, которые вы изучаете, можно в следующих статьях: 

[Добавление параметров Wi-Fi для устройств с Android в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Добавление параметров Wi-Fi для выделенных и полностью управляемых устройств с Android Enterprise в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Добавление параметров Wi-Fi для устройств iOS и iPadOS в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Добавление параметров Wi-Fi для устройств с Windows 10 и более поздних версий в Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Добавление параметров Wi-Fi для устройств Windows в Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Распространенные проблемы**

**Я выполняю развертывание профиля Wi-Fi, который зависит от развернутого сертификата, указанного в профиле Wi-Fi. Однако в профилях конфигурации отображается состояние ошибки.**

Убедитесь, что устройство получило сертификат.

1. В Intune перейдите в раздел **Все устройства** и выберите устройство > **Конфигурация устройства**.

2. Убедитесь, что все ожидаемые профили указаны и в успешном состоянии.

3. При наличии промежуточных сертификатов в цепочке сертификатов для профиля Android убедитесь, что они развернуты на устройствах с Android.

    Чтобы проверить состояние сертификата, перейдите в раздел **Конфигурация устройств** > **Профили** > **Промежуточный центр сертификации Android** > **Свойства** > **Доверенный сертификат**.

Если по-прежнему будут возникать ошибки, см. разделы "Процедуры" и "Устранение неполадок". Дополнительные сведения см. в статье [Общие сведения об устранении неполадок профилей сертификатов SCEP в Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Выполнено развертывание профиля Wi-Fi на устройстве. Intune показывает, что все прошло успешно, но устройство не подключается к Wi-Fi.**

Статус «успешно» означает, что приложение Intune успешно развернуло профиль в настроенном состоянии. Однако эти конфигурации могут не соответствовать требованиям вашей сети и (или) проверки подлинности. Дополнительные сведения о попытках подключения см. в журналах службы инфраструктуры и проверки подлинности (на контроллере точек доступа Wi-Fi и сервере NPS/RADIUS). Чтобы собрать и просмотреть журналы, вам, возможно, придется обратиться к вашей группе сетевой инфраструктуры или стороннему поставщику Wi-Fi.
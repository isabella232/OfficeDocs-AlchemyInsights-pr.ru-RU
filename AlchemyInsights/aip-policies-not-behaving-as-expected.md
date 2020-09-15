---
title: 'AIP: политики не работают должным образом'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663202"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: политики не работают должным образом

Служба Azure Information Protection. политики не работают должным образом; см. рекомендации по различным проблемам политик в следующих статьях.

1. При возникновении проблем с визуальной маркировкой см. статью[Когда применяется визуальная маркировка](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. При возникновении проблем с автоматическим присвоением метки см. статью [Как настроить условия для автоматической и рекомендуемой классификации для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и [Какие типы конфиденциальной информации искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. При возникновении проблем с защитой Native/Pfile см. статью [Конфигурация API для файлов](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Убедитесь в том, используете ли вы политики в области, которые не настроены должным образом, в статье [Как настроить политику Azure Information Protection для отдельных пользователей с помощью политик области](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Если автоматическое присвоение метки не работает в Outlook при прикреплении помеченного документа, то убедитесь в том, что свойство DRMEncryptProperty не задано, как описано в статье: [Параметры реестра IRM для безопасности](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Если проблемы не устраняются, то соберите клиентские журналы Azure Information Protection и вложите экспортированные журналы в этот запрос в службу поддержки.

1. Откройте документ Office или создайте новое сообщение электронной почты в Outlook.
2. Нажмите **Защитаt/Конфиденциальность** > **Справка и отзывы**.
3. Нажмите **Экспорт журналов**.
4. Сохраните журналы в выбранном расположении и вложите их в этот запрос в службу поддержки.

Дополнительные ресурсы:

- [Настройка метки для визуальной маркировки в Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Обзор документации Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Использование меток конфиденциальности в приложениях Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)


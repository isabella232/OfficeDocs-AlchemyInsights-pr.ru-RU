---
title: Автоматическая классификация не работает должным образом с клиентом AIP.
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820911"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматическая классификация не работает должным образом с клиентом AIP.

Если автоматическая классификация не работает должным образом, то воспользуйтесь следующими рекомендациями:

1. При возникновении проблем с автоматическим присвоением метки см. статью [Как настроить условия для автоматической и рекомендуемой классификации в Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) а [Какие типы конфиденциальной информации искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Убедитесь в том, используете ли вы политики в области, которые не настроены должным образом, в статье [Как настроить политику Azure Information Protection для отдельных пользователей с помощью политик области](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Если автоматическое присвоение метки не работает в Outlook при прикреплении помеченного документа, то убедитесь в том, что значение `DRMEncryptProperty` не задано, как описано в статье: [Параметры реестра IRM для безопасности](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Если вы использовали [встроенные типы данных](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) для своей политики Azure Information Protection, то проверьте, соответствует ли ваш контент ожидаемому формату.
5. Проверьте, правильно ли настроена метка для значения **Автоматическое** или **Рекомендованное**. (**Автоматическое** присвоение метки доступно для всех приложений Microsoft 365, при этом **Рекомендованное** присвоение метки доступно для всех приложений Microsoft 365, исключая Outlook.)
6. Вы не можете использовать автоматическую классификацию для документов и сообщений электронной почты, которым ранее была присвоена метка вручную или которым ранее автоматически была присвоена метка классификации более высокого уровня.  Дополнительные сведения приведены в статье [Применение автоматических или рекомендованных меток](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Если проблемы не устраняются, то соберите клиентские журналы Azure Information Protection и вложите экспортированные журналы в свой запрос в службу поддержки. Чтобы экспортировать журналы Azure Information Protection:
    - Откройте документ Office или создайте новое сообщение электронной почты в Outlook.
    - Нажмите **Защитаt/Конфиденциальность** > **Справка и отзывы**.
    - Нажмите **Экспорт журналов**.
    - Сохраните журналы в выбранном расположении и вложите их в запрос в службу поддержки.

Дополнительные сведения:

- [Настройка условий для автоматической и рекомендуемой классификации для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Пошаговые инструкции для распространенных сценариев, в которых используется Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Обзор документации Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Обзор подписок и функций Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Требования для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).
- [Краткое учебное руководство по Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Скачать клиента Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)

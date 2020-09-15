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
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="3f53d-102">AIP: политики не работают должным образом</span><span class="sxs-lookup"><span data-stu-id="3f53d-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="3f53d-103">Служба Azure Information Protection. политики не работают должным образом; см. рекомендации по различным проблемам политик в следующих статьях.</span><span class="sxs-lookup"><span data-stu-id="3f53d-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="3f53d-104">При возникновении проблем с визуальной маркировкой см. статью[Когда применяется визуальная маркировка](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="3f53d-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="3f53d-105">При возникновении проблем с автоматическим присвоением метки см. статью [Как настроить условия для автоматической и рекомендуемой классификации для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и [Какие типы конфиденциальной информации искать](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="3f53d-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="3f53d-106">При возникновении проблем с защитой Native/Pfile см. статью [Конфигурация API для файлов](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="3f53d-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="3f53d-107">Убедитесь в том, используете ли вы политики в области, которые не настроены должным образом, в статье [Как настроить политику Azure Information Protection для отдельных пользователей с помощью политик области](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="3f53d-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="3f53d-108">Если автоматическое присвоение метки не работает в Outlook при прикреплении помеченного документа, то убедитесь в том, что свойство DRMEncryptProperty не задано, как описано в статье: [Параметры реестра IRM для безопасности](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="3f53d-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="3f53d-109">Если проблемы не устраняются, то соберите клиентские журналы Azure Information Protection и вложите экспортированные журналы в этот запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="3f53d-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="3f53d-110">Откройте документ Office или создайте новое сообщение электронной почты в Outlook.</span><span class="sxs-lookup"><span data-stu-id="3f53d-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="3f53d-111">Нажмите **Защитаt/Конфиденциальность** > **Справка и отзывы**.</span><span class="sxs-lookup"><span data-stu-id="3f53d-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="3f53d-112">Нажмите **Экспорт журналов**.</span><span class="sxs-lookup"><span data-stu-id="3f53d-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="3f53d-113">Сохраните журналы в выбранном расположении и вложите их в этот запрос в службу поддержки.</span><span class="sxs-lookup"><span data-stu-id="3f53d-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="3f53d-114">Дополнительные ресурсы:</span><span class="sxs-lookup"><span data-stu-id="3f53d-114">Additional resources:</span></span>

- [<span data-ttu-id="3f53d-115">Настройка метки для визуальной маркировки в Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3f53d-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="3f53d-116">Обзор документации Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3f53d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3f53d-117">Использование меток конфиденциальности в приложениях Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3f53d-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)


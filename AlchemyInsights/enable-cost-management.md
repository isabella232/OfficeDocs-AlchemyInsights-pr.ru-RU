---
title: Включение управления затратами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599083"
---
# <a name="enable-cost-management"></a>Включение управления затратами

**Что означает, что затраты для вашей организации отключены?**

Организации, использующие учетные записи с корпоративным соглашением (EA) или Microsoft Customer Agreement (MCA), могут отключить доступ к сведениям о затратах и ценах.

После входа на портал Azure они могут использовать API выставления счетов для программного получения накладных (после выбора) и сведений об использовании.

**Как разрешить дополнительным пользователям получать доступ к счетам**

1. Перейдите к **колонке подписки** на портале Azure.
2. Выберите **счета** , а затем **доступ к счетам**.
3. Включите доступ, а затем сохраните изменения, чтобы разрешить пользователям в ролях с уровнями подписки загружать накладные.

> [!NOTE]
> Администратор учетной записи также может настроить для выставления счетов, отправляемых через электронную почту. Чтобы узнать больше, ознакомьтесь со [статьей получение счета по электронной почте](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Добавление пользователей в роль читателя выставления счетов**

1. Перейдите к **колонке подписки** на портале Azure.
2. Выберите **Управление доступом (IAM)** , а затем нажмите кнопку **Добавить**.
3. Выберите **средство "читатель выставления счетов** " на странице " **Выбор роли** ".
4. Введите адрес электронной почты пользователя, которого требуется пригласить, а затем нажмите кнопку **ОК** , чтобы отправить приглашение.
5. Следуйте инструкциям, приведенным в разделе приглашение, для входа в качестве средства чтения выставления счетов. Для получения дополнительных сведений обратитесь [к разделу предоставление доступа для выставления счетов](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Рекомендуемые документы**

- [Включение представлений DA и АО с помощью портала EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Затраты, включенные в управление затратами](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Поддерживаемые предложения Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Просмотр затрат в анализе затрат](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Предоставление доступа к сведениям о выставлении счетов](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Проверка доступа к соглашению о клиентах корпорации Майкрософт](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)







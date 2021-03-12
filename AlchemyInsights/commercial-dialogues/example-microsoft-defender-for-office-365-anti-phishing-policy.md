---
title: Пример политики защиты от фишинга Microsoft Defender для Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737874"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="eec75-102">Пример политики защиты от фишинга Microsoft Defender для Office 365</span><span class="sxs-lookup"><span data-stu-id="eec75-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="eec75-103">Эти параметры позволяют политику под названием *Домен и CEO*.</span><span class="sxs-lookup"><span data-stu-id="eec75-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="eec75-104">Эта политика обеспечивает защиту пользователя и домена от обезличения, а затем применяет политику ко всем электронным письмам, полученным пользователями в домене.</span><span class="sxs-lookup"><span data-stu-id="eec75-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="eec75-105">Сначала добавьте следующую информацию для создания политики:</span><span class="sxs-lookup"><span data-stu-id="eec75-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="eec75-106">**Имя**: Описание **домена** и ceo: гарантирует, что генеральный директор и ваш домен не будут обезличены.</span><span class="sxs-lookup"><span data-stu-id="eec75-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="eec75-107">**Применяется к**: Выберите **домен получателя**.</span><span class="sxs-lookup"><span data-stu-id="eec75-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="eec75-108">В **любом из них** выберите **выберите** и выберите домен.</span><span class="sxs-lookup"><span data-stu-id="eec75-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="eec75-109">Выберите **+ Добавить**.</span><span class="sxs-lookup"><span data-stu-id="eec75-109">Select **+ Add**.</span></span> <span data-ttu-id="eec75-110">Выберите контрольный ящик рядом с именем домена в списке (например, *contoso.com),* а затем выберите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="eec75-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="eec75-111">Нажмите кнопку **Готово**.</span><span class="sxs-lookup"><span data-stu-id="eec75-111">Select **Done**.</span></span>
- <span data-ttu-id="eec75-112">После создания политики можно настроить политику с помощью следующих параметров:</span><span class="sxs-lookup"><span data-stu-id="eec75-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="eec75-113">**Добавление пользователей для защиты:** В этом примере добавьте как минимум адрес электронной почты генерального директора.</span><span class="sxs-lookup"><span data-stu-id="eec75-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="eec75-114">**Добавление доменов для защиты:** Добавьте организационный домен, который включает офис генерального директора.</span><span class="sxs-lookup"><span data-stu-id="eec75-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="eec75-115">**Выберите действия:** **Если** электронная почта отправляется обезличенным пользователем, выберите перенаправление сообщения на другой адрес электронной почты, а затем введите адрес электронной почты администратора безопасности (например, *securityadmin@contoso.com).*</span><span class="sxs-lookup"><span data-stu-id="eec75-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="eec75-116">Если **электронная почта отправляется с помощью обезличенных доменов,** выберите карантин **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="eec75-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="eec75-117">**Аналитика почтовых ящиков.** По умолчанию этот параметр выбирается при создании новой политики защиты от фишинга.</span><span class="sxs-lookup"><span data-stu-id="eec75-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="eec75-118">Для достижения наилучших результатов оставьте значение **Вкл.**</span><span class="sxs-lookup"><span data-stu-id="eec75-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="eec75-119">**Добавление надежных отправителей и доменов:** В этом примере не нужно определять переопределения.</span><span class="sxs-lookup"><span data-stu-id="eec75-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="eec75-120">После просмотра параметров выберите **Создать** эту политику или **сохранить,** если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="eec75-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="eec75-121">Дополнительные новости см. в веб-сайте Политики защиты от фишинга [в Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)</span><span class="sxs-lookup"><span data-stu-id="eec75-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>

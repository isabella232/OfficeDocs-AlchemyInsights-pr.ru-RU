---
title: Сертификат Apple MDM Push не настроен
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431646"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="2415f-102">Сертификат Apple MDM Push не настроен</span><span class="sxs-lookup"><span data-stu-id="2415f-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="2415f-103">Сертификат Apple MDM Push (также называемый сертификатом службы push-уведомлений Apple (APNs)) для вашей подписки не настроен.</span><span class="sxs-lookup"><span data-stu-id="2415f-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="2415f-104">Без настроенного сертификата Apple MDM Push невозможно зарегистрировать устройства с iOS и MacOS, а также управлять ими.</span><span class="sxs-lookup"><span data-stu-id="2415f-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="2415f-105">После добавления этого сертификата в Intune пользователи смогут установить приложение корпоративного портала, чтобы зарегистрировать свои устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="2415f-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="2415f-106">Нажмите кнопку **"Принимаю".**,</span><span class="sxs-lookup"><span data-stu-id="2415f-106">Select **"I agree."**</span></span> <span data-ttu-id="2415f-107">чтобы предоставить Microsoft разрешение на отправку данных в Apple.</span><span class="sxs-lookup"><span data-stu-id="2415f-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="2415f-108">Щелкните **Скачать запрос CSR** для подписи сертификата Intune, необходимый для создания сертификата Apple MDM Push.</span><span class="sxs-lookup"><span data-stu-id="2415f-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="2415f-109">Этот файл нужен для запроса сертификата отношения доверия на портале Apple Push Certificates.</span><span class="sxs-lookup"><span data-stu-id="2415f-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="2415f-110">Щелкните **Создать свой сертификат MDM Push**, чтобы перейти на портал Apple Push Certificates.</span><span class="sxs-lookup"><span data-stu-id="2415f-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="2415f-111">Войдите с помощью идентификатора Apple ID своей компании и выберите пункт **Создать сертификат**.</span><span class="sxs-lookup"><span data-stu-id="2415f-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="2415f-112">Нажмите кнопку **Выбрать файл**, выберите файл запроса подписи сертификата и нажмите **Добавить**.</span><span class="sxs-lookup"><span data-stu-id="2415f-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="2415f-113">На странице подтверждения выберите **Скачать**, чтобы скачать файл сертификата (.pem) и сохранить его у себя.</span><span class="sxs-lookup"><span data-stu-id="2415f-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="2415f-114">**Примечание**. Сертификат связан с идентификатором Apple ID, использовавшимся при его создании.</span><span class="sxs-lookup"><span data-stu-id="2415f-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="2415f-115">Для управленческих задач рекомендуется использовать идентификатор Apple ID компании, а также обеспечить проверку почтового ящика несколькими людьми или пользоваться списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="2415f-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="2415f-116">Никогда не используйте личный идентификатор Apple ID.</span><span class="sxs-lookup"><span data-stu-id="2415f-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="2415f-117">Используйте один и тот же идентификатор Apple ID для продления сертификата Apple Push каждые 12 месяцев.</span><span class="sxs-lookup"><span data-stu-id="2415f-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="2415f-118">Введите идентификатор Apple ID, который был использован для создания сертификата Apple MDM Push.</span><span class="sxs-lookup"><span data-stu-id="2415f-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="2415f-119">Запишите этот идентификатор в качестве напоминания для того момента, когда потребуется продлить сертификат.</span><span class="sxs-lookup"><span data-stu-id="2415f-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="2415f-120">Перейдите к файлу сертификата (.pem), нажмите кнопку **Открыть** и выберите **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="2415f-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="2415f-121">Этот сертификат позволит Intune регистрировать устройства Apple и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="2415f-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>
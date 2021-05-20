---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544591"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f0116-102">Оповещение сообщений электронной почты из "Фишинг доставлено из-за политики переопределения клиента или пользователя"</span><span class="sxs-lookup"><span data-stu-id="f0116-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f0116-103">Политика оповещений по умолчанию с именем "Фишинг доставлена из-за переопределения клиента или пользователя" была выкатана для клиентов с лицензиями Microsoft Defender для Office 365 P1 и P2.</span><span class="sxs-lookup"><span data-stu-id="f0116-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="f0116-104">Если вы получили это оповещение, ниже следуют действия по расследованию:</span><span class="sxs-lookup"><span data-stu-id="f0116-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f0116-105">В сообщении оповещений нажмите **кнопку Просмотр** оповещений, чтобы перейти на страницу **Оповещения** в Центре & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f0116-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f0116-106">Выберите оповещение, чтобы просмотреть **список** сообщений или **просмотреть сообщения в Explorer.**</span><span class="sxs-lookup"><span data-stu-id="f0116-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f0116-107">Оба этих параметра содержат сведения о сообщении, в котором содержится ID сообщения.</span><span class="sxs-lookup"><span data-stu-id="f0116-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f0116-108">Обратите внимание, что ссылка Обозреватель угроз автоматически фильтрует сообщения, которые соответствуют критериям оповещения.</span><span class="sxs-lookup"><span data-stu-id="f0116-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f0116-109">Возможно, потребуется настроить фильтр дат в Обозревателе угроз.</span><span class="sxs-lookup"><span data-stu-id="f0116-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f0116-110">Сообщение фишинга было доставлено из-за переопределения вручную:</span><span class="sxs-lookup"><span data-stu-id="f0116-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f0116-111">Разрешенный отправитель или домен, установленный пользователем.</span><span class="sxs-lookup"><span data-stu-id="f0116-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f0116-112">Разрешенный отправитель или домен, установленный администратором в политике борьбы со спамом.</span><span class="sxs-lookup"><span data-stu-id="f0116-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f0116-113">Разрешенный IP-адрес в политике фильтра подключения.</span><span class="sxs-lookup"><span data-stu-id="f0116-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f0116-114">Правило потока почты (также известное как правило транспорта), настроенное для допуска сообщений.</span><span class="sxs-lookup"><span data-stu-id="f0116-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f0116-115">Если вы считаете, что сообщение было неправильно помечено как фишинг, используйте надстройку Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) для отправки образцов сообщений в Корпорацию Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f0116-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>

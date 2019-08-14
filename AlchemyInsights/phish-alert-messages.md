---
title: 2491 оповещение сообщения электронной почты из политики "фишинг доставлено из-за клиента или переопределение пользователя"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391484"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="fa979-102">Оповещение о сообщениях электронной почты из политики "фишинг доставлено из-за клиента или переопределение пользователя"</span><span class="sxs-lookup"><span data-stu-id="fa979-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="fa979-103">В клиентах, использующих лицензии Office 365 ATP P1 и P2, было выполнено развертывание политики оповещений по умолчанию с именем "фишинг доставлено из-за клиента или переопределение пользователя".</span><span class="sxs-lookup"><span data-stu-id="fa979-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="fa979-104">Если вы получили это предупреждение, выполните следующие действия для изучения:</span><span class="sxs-lookup"><span data-stu-id="fa979-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="fa979-105">Из сообщения оповещения щелкните **Просмотр оповещения** , чтобы перейти на страницу **оповещения** центра безопасности & соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="fa979-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="fa979-106">Выберите оповещение, чтобы увидеть возможность **просмотра списка сообщений** или **просмотра сообщений в проводнике**.</span><span class="sxs-lookup"><span data-stu-id="fa979-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="fa979-107">Оба эти параметра помогут получить сведения о сообщении, которое включает идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="fa979-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="fa979-108">Обратите внимание, что ссылка "Обозреватель угроз" автоматически фильтрует сообщения, которые отвечают условиям оповещения.</span><span class="sxs-lookup"><span data-stu-id="fa979-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="fa979-109">Возможно, вам потребуется настроить фильтр дат в обозревателе угроз.</span><span class="sxs-lookup"><span data-stu-id="fa979-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="fa979-110">Сообщение фишинга доставлено из-за переопределения, настроенного вручную:</span><span class="sxs-lookup"><span data-stu-id="fa979-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="fa979-111">Разрешенный отправитель или домен, установленный пользователем.</span><span class="sxs-lookup"><span data-stu-id="fa979-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="fa979-112">Разрешенный отправитель или домен, заданный администратором в политике защиты от нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="fa979-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="fa979-113">Разрешенный IP-адрес в политике фильтрации подключений.</span><span class="sxs-lookup"><span data-stu-id="fa979-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="fa979-114">Правило поток обработки почты (также называемое правилом транспорта), которое разрешает сообщения в.</span><span class="sxs-lookup"><span data-stu-id="fa979-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="fa979-115">Если вы считаете, что сообщение ошибочно помечено как фишинг, используйте [надстройку отчета](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook для отправки примеров сообщений в корпорацию Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fa979-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>

---
title: Создание политик меток АДМИНИСТРАТИВной установки
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732188"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="b28bb-102">Создание политик меток АДМИНИСТРАТИВной установки</span><span class="sxs-lookup"><span data-stu-id="b28bb-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="b28bb-103">Метки Azure Information Protection (точка административной защиты) можно использовать с полным диапазоном данных, которые Организация обычно создает и сохраняет, начиная с наименьшей классификации персональных данных, с максимальной классификацией строго конфиденциальных данных.</span><span class="sxs-lookup"><span data-stu-id="b28bb-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="b28bb-104">Политики Azure Information Protection применяются к классическому клиенту Azure Information Protection (точка административной защиты), а не к  [клиенту единой метки административного административного](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)имени.</span><span class="sxs-lookup"><span data-stu-id="b28bb-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="b28bb-105">В политике АДМИНИСТРАТИВной установки можно настроить несколько элементов, в том числе следующие:</span><span class="sxs-lookup"><span data-stu-id="b28bb-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="b28bb-106">Параметр, с помощью которого метка позволит администраторам или пользователям классифицировать и защищать (необязательно) документы и сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="b28bb-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="b28bb-107">Возможность применения классификации при сохранении документов и отправке электронной почты</span><span class="sxs-lookup"><span data-stu-id="b28bb-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="b28bb-108">Возможность автоматической подписи сообщения электронной почты на основе вложений.</span><span class="sxs-lookup"><span data-stu-id="b28bb-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="b28bb-109">Возможность указать, отображается ли панель защиты информации в приложениях Office</span><span class="sxs-lookup"><span data-stu-id="b28bb-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="b28bb-110">Дополнительные параметры и сведения о политиках Azure Information Protection: [Обзор политики Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="b28bb-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="b28bb-111">Другие полезные ресурсы, посвященные политикам АДМИНИСТРАТИВной установки, приведены ниже.</span><span class="sxs-lookup"><span data-stu-id="b28bb-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="b28bb-112">Руководство: настройка параметров политики Azure Information Protection и создание новой метки</span><span class="sxs-lookup"><span data-stu-id="b28bb-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b28bb-113">Настройка политики Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b28bb-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="b28bb-114">Создание и настройка меток конфиденциальности и соответствующих политик</span><span class="sxs-lookup"><span data-stu-id="b28bb-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="b28bb-115">Пошаговые инструкции для распространенных сценариев, в которых используется Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b28bb-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="b28bb-116">Обзор документации Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b28bb-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- <span data-ttu-id="b28bb-117">[Требования для Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="b28bb-117">[Requirements for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span></span>  
- [<span data-ttu-id="b28bb-118">Краткое учебное руководство по Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b28bb-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b28bb-119">Скачать клиента Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b28bb-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
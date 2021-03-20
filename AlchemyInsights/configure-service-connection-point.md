---
title: Настройка точки подключения службы (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898066"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="8eca4-102">Настройка точки подключения службы (SCP)</span><span class="sxs-lookup"><span data-stu-id="8eca4-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="8eca4-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="8eca4-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="8eca4-104">**Причина**: не удается прочитать объект SCP и получить сведения о клиенте Azure AD</span><span class="sxs-lookup"><span data-stu-id="8eca4-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="8eca4-105">**Решение**: обратитесь к разделу [Настройка точки подключения службы](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="8eca4-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="8eca4-106">**План действий**</span><span class="sxs-lookup"><span data-stu-id="8eca4-106">**Action plan**</span></span>

- <span data-ttu-id="8eca4-107">Проверьте, получен ли устройством объект групповой политики (GPO) для контролируемой проверки.</span><span class="sxs-lookup"><span data-stu-id="8eca4-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="8eca4-108">Убедитесь, что GPO создал ключи реестра.</span><span class="sxs-lookup"><span data-stu-id="8eca4-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="8eca4-109">Убедитесь, что у вас есть 2 ключа, созданных с помощью вашего ИД каталога и домена onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="8eca4-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="8eca4-110">**Настройка параметра реестра на стороне клиента для SCP**</span><span class="sxs-lookup"><span data-stu-id="8eca4-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="8eca4-111">Используйте следующий пример для создания объекта групповой политики (GPO) для развертывания параметра реестра, который настраивает запись SCP в реестре ваших устройств.</span><span class="sxs-lookup"><span data-stu-id="8eca4-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="8eca4-112">Откройте консоль управления групповыми политиками и создайте новый GPO в вашем домене.</span><span class="sxs-lookup"><span data-stu-id="8eca4-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="8eca4-113">Дайте новому GPO имя (например, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="8eca4-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="8eca4-114">Отредактируйте GPO и найдите следующий путь: **Конфигурация компьютера > Параметры > Параметры Windows > Реестр**.</span><span class="sxs-lookup"><span data-stu-id="8eca4-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="8eca4-115">Щелкните правой кнопкой мыши **Реестр** и выберите **Создать > Элемент реестра**.</span><span class="sxs-lookup"><span data-stu-id="8eca4-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="8eca4-116">На вкладке **Общие** настройте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="8eca4-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="8eca4-117">**Действие**: обновление</span><span class="sxs-lookup"><span data-stu-id="8eca4-117">**Action**: Update</span></span>
    
- <span data-ttu-id="8eca4-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="8eca4-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="8eca4-119">**Путь к разделу**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="8eca4-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="8eca4-120">**Имя значения**: TenantId</span><span class="sxs-lookup"><span data-stu-id="8eca4-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="8eca4-121">Тип значения: **REG_SZ**</span><span class="sxs-lookup"><span data-stu-id="8eca4-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="8eca4-122">**Значение**: GUID или ИД каталога экземпляра Azure AD (это значение можно найти на портале **Azure > Azure Active Directory > Свойства > ИД каталога**)</span><span class="sxs-lookup"><span data-stu-id="8eca4-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="8eca4-123">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="8eca4-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="8eca4-124">Щелкните правой кнопкой мыши **Реестр** и выберите **Создать > Элемент реестра**.</span><span class="sxs-lookup"><span data-stu-id="8eca4-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="8eca4-125">На вкладке **Общие** настройте следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="8eca4-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="8eca4-126">**Действие**: обновление</span><span class="sxs-lookup"><span data-stu-id="8eca4-126">**Action**: Update</span></span>
    
- <span data-ttu-id="8eca4-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="8eca4-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="8eca4-128">**Путь к разделу**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="8eca4-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="8eca4-129">**Имя значения**: TenantName</span><span class="sxs-lookup"><span data-stu-id="8eca4-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="8eca4-130">Тип значения: **REG_SZ**</span><span class="sxs-lookup"><span data-stu-id="8eca4-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="8eca4-131">**Значение**: ваше проверенное доменное имя, если вы используете интегрированную среду, например AD FS.</span><span class="sxs-lookup"><span data-stu-id="8eca4-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="8eca4-132">Проверенное доменное имя или onmicrosoft.com доменное имя (например, contoso.onmicrosoft).com, если вы используете управлевую среду</span><span class="sxs-lookup"><span data-stu-id="8eca4-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="8eca4-133">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="8eca4-133">Click **OK**.</span></span>

7. <span data-ttu-id="8eca4-134">Закройте редактор только что созданного GPO.</span><span class="sxs-lookup"><span data-stu-id="8eca4-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="8eca4-135">Привяжите только что созданный GPO к нужному OU, содержащему компьютеры, объединенные доменом и принадлежащие к вашей группе контролируемого развертывания.</span><span class="sxs-lookup"><span data-stu-id="8eca4-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="8eca4-136">Дополнительные сведения см. в статьях [Управляемая проверка гибридного соединения Azure AD — Azure AD |  Документация Майкрософт](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) и [Устранение неполадок с гибридными устройствами, подключенными к Azure Active Directory| Документация Майкрософт](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="8eca4-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>










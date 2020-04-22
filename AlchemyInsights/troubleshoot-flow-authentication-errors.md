---
title: Устранение ошибок проверки подлинности для последовательности
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759741"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="0fec9-102">Устранение ошибок проверки подлинности для последовательности</span><span class="sxs-lookup"><span data-stu-id="0fec9-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="0fec9-103">Во многих случаях потоки не проходят из-за ошибки проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0fec9-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="0fec9-104">Если у вас возникли ошибки такого типа, сообщение об ошибке содержит "несанкционированный", или отображается код ошибки 401 или 403.</span><span class="sxs-lookup"><span data-stu-id="0fec9-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="0fec9-105">Обычно для устранения ошибки проверки подлинности можно выполнить обновление подключения:</span><span class="sxs-lookup"><span data-stu-id="0fec9-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="0fec9-106">В верхней части веб-портала щелкните значок шестеренки, чтобы открыть меню Параметры, а затем щелкните **подключения**.</span><span class="sxs-lookup"><span data-stu-id="0fec9-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="0fec9-107">Перейдите к подключению, для которого вы видели сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0fec9-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="0fec9-108">Рядом с подключением щелкните или коснитесь ссылки **проверить пароль** в сообщении о том, что проверка подлинности для подключения не выполняется.</span><span class="sxs-lookup"><span data-stu-id="0fec9-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="0fec9-109">Проверьте учетные данные, следуя появившимся инструкциям, вернитесь к ошибке выполнения потока, а затем щелкните или нажмите кнопку Повторная **Передача**.</span><span class="sxs-lookup"><span data-stu-id="0fec9-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="0fec9-110">Дополнительные сведения можно найти [в разделе Устранение неполадок, связанных с процессом](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="0fec9-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  


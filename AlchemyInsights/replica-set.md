---
title: Набор реплик
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110693"
---
# <a name="replica-set"></a>Набор реплик

AADDS также называется управляемым доменом. На самом деле это два контроллера домена, которые запускаются и поддерживаются backend. Два DCs включают один основной DC и один DC репликации. Резервное копирование в AADDS (управляемом домене) — это автоматизированный процесс, управляемый платформой Azure. В случае проблемы с управляемым доменом поддержка Azure может помочь вам в восстановлении из резервного копирования.

Каждая реплика создается в виртуальной сети. Каждая виртуальная сеть должна быть вглядеться во все другие виртуальные сети, в которых размещен набор реплик управляемых доменов. Эта конфигурация создает топологию сетевой сети, которая поддерживает репликацию каталогов. Виртуальная сеть может поддерживать несколько наборов реплик при условии, что каждый набор реплик находится в другой виртуальной подсети.

Дополнительные сведения о наборе реплик см. в [материале "Реплика концепций".](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)

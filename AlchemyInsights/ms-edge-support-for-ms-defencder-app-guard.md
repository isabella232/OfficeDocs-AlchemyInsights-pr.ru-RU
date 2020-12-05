---
title: Поддержка Microsoft Edge Application Guard для защитника Microsoft
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576634"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Поддержка Microsoft Edge Application Guard для защитника Microsoft

Приложение Application Guard предназначено для Windows 10 и Microsoft EDGE, которое позволяет пользователю перемещаться по недоверенному сайту из изолированного контейнера с поддержкой Hyper-V, отделенного от операционной системы узла.

Администратор предприятия определяет список надежных веб-сайтов, облачных ресурсов и внутренних сетей. Когда пользователь посещает сайт, которого нет в списке, Microsoft Edge откроет сайт в контейнере. Это означает, что если сайт станет вредоносным, ведущий компьютер останется защищенным, а злоумышленник не получит доступ к корпоративным данным.

Установка расширений в контейнере поддерживается в Microsoft Edge версии 81, и ее можно контролировать с помощью политики. Адрес Упдатеурл, который будет использоваться в политике Екстенсионинсталлфорцелист, должен быть добавлен в качестве нейтрального ресурса в политиках сетевой изоляции, используемых Application Guard.

Дополнительные сведения см. в разделе [Поддержка Microsoft Edge для Application Guard в защитнике Microsoft](https://go.microsoft.com/fwlink/?linkid=2134229).

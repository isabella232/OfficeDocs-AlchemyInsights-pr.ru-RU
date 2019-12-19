---
title: Устранение неполадок существующего монитора
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738581"
---
# <a name="troubleshoot-an-existing-monitor"></a>Устранение неполадок существующего монитора

Воспользуйтесь этими решениями, чтобы устранить неполадки с монитором. 

**Обновите экран монитора:**

Одновременно используйте следующие клавиши: клавиша Windows + Ctrl + Shift + B. При этом будет обновлена связь с драйвером графической подсистемы. Мониторы мигают на мгновениях и будут возвращаться через несколько секунд.

**Устранение неполадок оборудования монитора:**

1. Отсоедините кабель, соединяющий компьютер с монитором, и снова подключите его.
2. Отключите все несущественные устройства от компьютера (например, адаптеры или стыковочные устройства).

**Если вы недавно установили обновление на компьютере, вы можете откатить свой драйвер экрана:**

1. Нажмите кнопку **Пуск**, введите **Диспетчер устройств**и выберите **Диспетчер устройств** из результатов.
2. Разверните раздел **Видеоадаптеры** , щелкните правой кнопкой мыши видеоадаптер, смешивать и выберите **свойства**.
3. Перейдите на вкладку **Driver (драйвер** ) и выберите пункт **вернуть драйвер**. <br>
Примечание. Если этот параметр недоступен или неактивен, выберите пункт **нет** в списке ниже, чтобы перейти к следующему шагу.
4. Для вступления изменений в силу может потребоваться перезагрузка компьютера.

**Удалите и переустановите драйвер экрана.**

1. Нажмите кнопку **Пуск**, введите **Диспетчер устройств**и выберите **Диспетчер устройств** из результатов.
2. Разверните раздел **Видеоадаптеры** , щелкните правой кнопкой мыши видеоадаптер смешивать и выберите пункт **удалить устройство**. 
3. Установите флажок рядом с пунктом **удалить драйвер для этого устройства** и нажмите кнопку **Удалить**.<br>
Примечание. вам может быть предложено перезапустить компьютер на этом этапе. Перед перезагрузкой обязательно запишите остальные инструкции.
4. Снова откройте Диспетчер устройств.
5. Разверните раздел **адаптеры отображения** , щелкните правой кнопкой мыши видеоадаптер и выберите команду **Обновить драйвер**.
6. Выберите **автоматически Поиск по драйверу обновления** и следуйте инструкциям по установке.
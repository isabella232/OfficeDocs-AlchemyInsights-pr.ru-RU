---
title: Невозможно добавить учетную запись после перехода на macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446746"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Невозможно добавить учетную запись после перехода на macOS 11.6 Big Sur

После перехода на macOS 11.6 ваша рабочая или учебная учетная запись OneDrive либо ваша личная учетная запись OneDrive может не отображаться в списке учетных записей, и вы не сможете войти во вторую учетную запись из приложения.

Эта возникающая проблема связана с переходом на macOS 11.6. Пока проблема не будет устранена, вы можете получить доступ к содержимому OneDrive из веб-версии или со своего мобильного устройства. Корпорация Майкрософт взаимодействует с Apple для восстановления функций OneDrive.

Вы также можете запустить отсутствующий экземпляр OneDrive вручную с помощью терминала. 

**Примечание.** Это временное решение работает только до перезапуска OneDrive (вызванного перезагрузкой компьютера или обновлением приложения OneDrive).

Если отсутствующим экземпляром является личная учетная запись, откройте терминал и введите:

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Если отсутствующим экземпляром является рабочая или учебная учетная запись, откройте терминал и введите:

`open "/Applications/OneDrive.app" --new --args /client=Business1`


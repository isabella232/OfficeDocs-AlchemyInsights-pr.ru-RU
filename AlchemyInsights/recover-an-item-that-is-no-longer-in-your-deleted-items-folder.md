---
title: Восстановление элемента, который больше не находится в папке "Удаленные"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "7320"
ms.openlocfilehash: b6ac084ead88b090d6caab1405d5d96f24890ea7
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560713"
---
# <a name="recover-an-item-thats-no-longer-in-your-deleted-items-folder"></a>Восстановление элемента, который больше не находится в папке "Удаленные"

Если вы не можете найти элемент в папке "Удаленные", то в папке "элементы с возможностью восстановления" появится следующее место поиска. Это скрытая папка, в которую перемещаются элементы в следующих случаях:
- Они удаляются из папки "Удаленные".
- Папка "Удаленные" очищается либо политикой, установленной ИТ-администратором.
- Чтобы удалить элемент, выделите его и нажмите клавиши **SHIFT + DELETE**.

Для просмотра и восстановления элементов, перемещенных в папку "элементы с возможностью восстановления":
1. В браузере войдите в Outlook Web App, используя URL-адрес, предоставленный пользователем, который управляет электронной почтой вашей организации. Введите имя пользователя и пароль, а затем нажмите кнопку **войти**.
1. В списке папок электронной почты щелкните правой кнопкой мыши **Удаленные элементы**, а затем выберите команду **восстановить удаленные элементы..**..
1. При необходимости используйте поле поиска для поиска элемента, который требуется восстановить.
1. Найдя элемент, выберите его и нажмите кнопку **восстановить**.
   Восстановленные элементы перемещаются в расположение по умолчанию для каждого типа элементов.
    - Сообщения отправляются в папку "Входящие".
    - Элементы календаря отправляются в календарь.
    - Контакты отправляются в папку "Контакты".
    - Задачи перейдите в папку "задачи".

**Советы по восстановлению элементов в папке "элементы с возможностью восстановления"**

- Дата удаления элемента в папке "элементы с возможностью восстановления" заключается в том, что элемент был перемещен в папку "Удаленные". Это не дата перемещения элемента в папку "элементы с возможностью восстановления".
- Элементы в папке "элементы с возможностью восстановления" не имеют значков, поэтому все они выглядят очень похожими.
    - Если вы ищете контакт, ищите элемент с именем человека, но без строки темы.
    - Если вы ищете встречу в календаре, найдите элемент, для которого не задано имя пользователя или строка темы.
    - Если вы ищете контакт, встречу в календаре или задача ищет текст этого элемента.
- Чтобы восстановить несколько элементов, наведите указатель мыши на каждый элемент и установите флажок рядом с ним, нажмите кнопку **восстановить**. Кроме того, можно восстановить несколько смежных элементов, установив флажок для первого элемента, удерживая клавишу **SHIFT** , а затем установив флажок для последнего элемента. После выбора всех элементов нажмите кнопку **восстановить**.
- Вы можете удалить элементы из списка **Восстановление удаленных элементов** . Просто выберите элемент, а затем нажмите **очистить**. Если вы удаляете элемент, вы не сможете использовать восстановление удаленных элементов, чтобы вернуть его обратно. При очистке сообщения оно не удаляется из резервных копий, которые были сделаны до очистки.
- В Организации может быть указано, как долго элементы в папке "элементы с возможностью восстановления" доступны для восстановления. Например, может быть политика, которая удаляет все элементы в папке "Удаленные" в течение 30 дней и другую политику, которая позволяет восстанавливать элементы в папке "элементы с возможностью восстановления" в течение еще одного 14 дней.
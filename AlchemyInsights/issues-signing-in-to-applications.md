---
title: Ошибки при входе в приложения
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886905"
---
# <a name="issues-signing-in-to-applications"></a>Ошибки при входе в приложения

Чтобы найти причину проблемы или диагностировать ошибки, связанные со входом пользователя, выполните следующие действия:

1. Запустите [Диагностику входа](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Найдите событие, которое нужно проанализировать, указав сведения о пользователе, приложении, времени входа, идентификаторе запроса или корреляции.
3. Ознакомьтесь с результатами диагностики, отображающими подробные сведения о том, что произошло и какие действия нужно предпринять, чтобы внести изменения.

Ниже перечислены некоторые распространенные ошибки, которые могут возникнуть при входе в приложения:

1. Вы или пользователь **выполнили вход в службу Azure AD, но возникла непредвиденная ошибка.** См. статью [Непредвиденный запрос согласия при попытке войти в приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) и [Непредвиденная ошибка при предоставлении согласия приложению](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Вы или пользователь **вошли в приложение напрямую, но не может войти в него с помощью прямой ссылки на настраиваемом портале или панели доступа**: см. статью [Устранение неполадок со входом в приложение из Azure AD или Мои приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Вы или пользователь **выполнили вход в Azure AD, но приложение выдает сообщение об ошибке, которое не позволяет пользователю закончить процедуру входа**: проблема заключается в том, что приложение не приняло ответ, заданный Azure AD. Чтобы устранить неполадку, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error).
4. Вы или пользователь **не можете выполнить вход в приложение, не относящееся к галерее, для которого настроен единый вход с паролем**: чтобы устранить неполадки, следуйте [этим инструкциям](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso).
5. Вы или пользователь **не можете выполнить вход в приложение коллекции Azure AD, для которого настроен единый вход с паролем**: чтобы устранить неполадки, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso).
6. Вы или пользователь **не можете войти в приложение Microsoft**: чтобы устранить неполадки, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft).
7. Вы или пользователь **не можете выполнить вход в приложение, не относящееся к галерее, для которого настроен федеративный единый вход**: чтобы устранить неполадки, следуйте [этим инструкциям](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery).
8. Вы или пользователь **не можете выполнить вход в приложение коллекции Azure AD, для которого настроен федеративный единый вход**: чтобы устранить неполадки, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery).
9. Вы или пользователь **не можете войти в настраиваемое приложение**: чтобы устранить неполадки, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery).
10. Вы или пользователь **не можете войти в локальное приложение с помощью прокси-сервера Azure AD**: чтобы устранить неполадки, выполните [эти действия](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy).


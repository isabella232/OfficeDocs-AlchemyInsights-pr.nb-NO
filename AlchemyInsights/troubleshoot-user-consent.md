---
title: Feilsøke brukersamtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007907"
---
# <a name="troubleshoot-user-consent"></a>Feilsøke brukersamtykke

1. Du kan konfigurere hvordan sluttbrukere samtykker til programmer via Azure Portal eller PowerShell. Se [Innstillinger for brukersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for mer informasjon.
1. En administrator kan også bruke [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til å gi samtykke til delegerte tillatelser på vegne av én enkelt bruker. Hvis du vil ha mer informasjon, kan [du se Få tilgang på vegne av en bruker](https://docs.microsoft.com/graph/auth-v2-user).
1. [Feil med](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)brukersamtykke: Denne artikkelen omhandler feil som kan oppstå under prosessen med å samtykke til et program. Hvis du feilsøker uventede samtykkemeldinger som ikke inneholder feilmeldinger, kan du se [Godkjenningsscenarioer for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
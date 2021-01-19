---
title: Feilsøke bruker samtykke
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901635"
---
# <a name="troubleshoot-user-consent"></a>Feilsøke bruker samtykke

1. Du kan konfigurere hvordan slutt brukere samtykker til programmer gjennom Azure-portalen eller PowerShell. Se [bruker samtykke innstillinger](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for mer informasjon.
1. En administrator kan også bruke [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til å gi samtykke til delegert tilgang på vegne av en enkelt bruker. Hvis du vil ha mer informasjon, kan du se [få tilgang på vegne av en bruker](https://docs.microsoft.com/graph/auth-v2-user).
1. [Bruker samtykke feil](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): denne artikkelen omhandler feil som kan oppstå under prosessen med å sendes til et program. Hvis du feil søker ukjente bekreftelser på samtykker som ikke inneholder noen feil meldinger, kan du se [godkjennings scenarioer for Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
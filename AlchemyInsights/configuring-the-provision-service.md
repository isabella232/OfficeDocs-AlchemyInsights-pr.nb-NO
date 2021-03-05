---
title: Konfigurere klargjøringstjenesten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482873"
---
# <a name="configuring-the-provision-service"></a>Konfigurere klargjøringstjenesten

For at automatisert klargjøring av bruker skal fungere, krever Azure AD gyldig legitimasjon som tillater at den kobler seg til Workday Web Services API. I tillegg validerer knappen Test tilkobling på klargjøringsappen for Arbeidsdag til AD-bruker også om den kan koble til klargjøringsagenten for Azure AD Connect knyttet til AD-domenet.

Hvis Azure-portalen returnerer en feil når du lagrer legitimasjonen, følger du de anbefalte trinnene nedenfor:

1. Kontroller at du har konfigurert brukerkontoen for Workday Integration System som angitt i opplæringsdelen [Konfigurere integrasjonssystembruker i Arbeidsdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Kontroller at klargjøringsagenttjenesten for Azure AD Connect er oppe og kjører på den lokale Windows-serveren ved hjelp av tjenestebehandlingskonsollen. Du kan også kontrollere statusen til agenten i Azure Portal ved å klikke knappen Vis lokale agenter.
3. Kontroller at du skriver inn verdien for feltet Brukernavn for arbeidsdag ved hjelp av formatet username@workday-tenant-navn. Hvis navnet på arbeidsdagen-tenanten mangler, mislykkes godkjenningen for arbeidsdagen.
4. Hvis du konfigurerer integrering med Workday-implementering av tenanten, må du notere deg de planlagte nedetidstimene for Arbeidsdag-leieren. Arbeidsdagen har planlagt nedsatt tid for implementering av leiere over helger (vanligvis fra fredag kveld til lørdag morgen) og tilkoblingsfeil i dette nedetidsvinduet er et kjent problem som automatisk løses så snart implementeringen av tenantene er tilkoblet igjen.
5. I sjeldne tilfeller kan du også se denne feilen hvis passordet til integrasjonssystemets bruker endres på grunn av en leieroppdatering, eller hvis kontoen er låst eller har utløpt status. Kontroller statusen for integrasjonssystemet med workday-administratoren.

Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av bruker.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

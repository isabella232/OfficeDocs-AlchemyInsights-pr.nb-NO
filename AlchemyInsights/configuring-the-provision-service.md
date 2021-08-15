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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033287"
---
# <a name="configuring-the-provision-service"></a>Konfigurere klargjøringstjenesten

For at automatisert klargjøring av bruker skal fungere, krever Azure AD gyldig legitimasjon som tillater at den kobler til Workday Web Services API. Videre validerer Test tilkobling-knappen på Workday to AD User Provisioning-appen også om den er i stand til å koble til Azure AD Koble til Klargjøringsagent som er knyttet til AD-domenet.

Hvis Azure-portalen returnerer en feil når du lagrer legitimasjonen, følger du de anbefalte trinnene nedenfor:

1. Bekreft at du har konfigurert brukerkontoen for Workday Integration System som angitt i opplæringsdelen [Konfigurere integreringssystembruker i Arbeidsdag](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Bekreft at Azure AD Koble til Klargjøringsagenttjeneste er oppe og kjører på den lokale Windows-serveren ved hjelp av Tjenestebehandlingskonsollen. Du kan også kontrollere statusen til agenten i Azure-portalen ved å klikke knappen Vis lokale agenter.
3. Kontroller at du skriver inn verdien for «Arbeidsdag brukernavn»-feltet ved hjelp av formatet username@workday-tenant-name. Hvis navnet på arbeidsdagen-tenanten mangler, mislykkes arbeidsdaggodkjenningen.
4. Hvis du konfigurerer integreringen med Workday-implementerings tenanten, noterer du deg de planlagte nedetidstimene for Arbeidsdag-tenanten. Arbeidsdagen har planlagt nedetid for implementeringsleierne i helgene (vanligvis fra fredag kveld til lørdag morgen) og tilkoblingsfeil i dette nedetidsvinduet er et kjent problem som løses automatisk så snart implementeringsleierne er tilkoblet igjen.
5. I sjeldne tilfeller kan du også se denne feilen hvis passordet til integreringssystemets bruker ble endret på grunn av tenantoppdatering, eller hvis kontoen er låst eller utløpt. Kontroller statusen for Integreringssystem-brukeren med Workday-administratoren.

Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

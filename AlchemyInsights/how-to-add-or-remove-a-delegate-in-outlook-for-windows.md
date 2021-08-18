---
title: Slik legger du til eller fjerner en representant i Outlook for Windows
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
- "3800004"
- "7334"
ms.openlocfilehash: 8db800d5c23b4cc2057f94abaf357082914143d3
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329049"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Slik legger du til eller fjerner en representant i Outlook for Windows

Slik legger du til en representant Outlook for Windows: 

1. Klikk på **Fil-fanen** etterfulgt av **Konto Innstillinger**, og velg deretter **Representanttilgang**.
2. Klikk Legg **til**. Hvis **Legg** til ikke vises, kan det hende at det ikke finnes en aktiv tilkobling mellom Outlook og Exchange. Statuslinjen Outlook viser tilkoblingsstatusen.
3. Skriv inn navnet på personen du vil angi som representant, eller søk og velg navnet i listen over søkeresultater.

    **Obs!** Representanten må være en person i organisasjonens Exchange global adresseliste (GAL).
4. Klikk legg **til** etterfulgt av **OK**.
5. Godta standard **tillatelsesinnstillinger** i dialogboksen Representanttillatelser, eller velg egendefinerte tilgangsnivåer for Exchange mapper.

    - Hvis en representant bare trenger tillatelse til å arbeide med møteinvitasjoner og svar, er standard tillatelsesinnstillinger, for eksempel Representant, kopier av **møterelaterte** meldinger sendt til meg tilstrekkelig. Du kan la **innbokstillatelsesinnstillingen** være på **Ingen**. Møteinnkallelser og svar går direkte til representantens innboks.

    **Obs!** Representanten får som standard **redigeringstillatelse (kan lese, opprette** og endre elementer) til **Kalender-mappen.** Når representanten svarer på et møte på dine vegne, legges den automatisk til i **Kalender-mappen.**

5. Hvis du vil sende en melding for å varsle representanten om de endrede tillatelsene, merker du av for Send automatisk en melding til representant som **oppsummerer disse tillatelsene.**
6. Hvis du vil, merker du av **for Representanten kan se mine private elementer.**

    **Viktig!** Denne innstillingen påvirker alle Exchange mapper. Dette omfatter alle mappene E-post, Kontakter, Kalender, Oppgaver, Notater og Logg. Det er ikke mulig å gi tilgang til private elementer i bare angitte mapper.

7. Velg **OK**.

    **Obs!**
    - Meldinger som sendes med send på vegne av-tillatelsene, omfatter både representantens og navnene dine ved siden av **Fra**. Når en melding sendes med Send som-tillatelser, vises bare navnet ditt.
    - Når du har lagt til noen som representant, kan de legge Exchange postboksen til vedkommendes Outlook profil. Hvis du vil ha instruksjoner, kan du se Administrere en [annen persons e-post- og kalenderelementer](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Slik fjerner du en representant Outlook for Windows:

1. Klikk på **Fil-fanen.**
2. Klikk på **Konto Innstillinger** etterfulgt av **Representanttilgang**.
3. Velg navnet på representanten du vil endre tillatelser for, og klikk deretter Fjern **etterfulgt** av **OK**.

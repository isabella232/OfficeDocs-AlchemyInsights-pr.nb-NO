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
ms.openlocfilehash: ee54e2bcca4f4591b33ee805290192311f6cde09a9e453a813e9db328d19634d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945346"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Slik legger du til eller fjerner en representant i Outlook for Windows

Slik legger du til en representant Outlook for Windows: 

1. Klikk på **Fil-fanen** etterfulgt av **Konto Innstillinger**, og velg deretter **Representanttilgang**.
2. Klikk Legg **til**. Hvis **Legg** til ikke vises, finnes det kanskje ikke en aktiv tilkobling mellom Outlook og Exchange. Statuslinjen Outlook viser tilkoblingsstatusen.
3. Skriv inn navnet på personen du vil angi som representant, eller søk og velg navnet i listen over søkeresultater.

    > [!NOTE]
    > Representanten må være en person i organisasjonens Exchange global adresseliste (GAL).
4. Klikk legg **til** etterfulgt av **OK**.
5. Godta standard **tillatelsesinnstillinger** i dialogboksen Representanttillatelser, eller velg egendefinerte tilgangsnivåer for Exchange mapper.

    - Hvis en representant bare trenger tillatelse til å arbeide med møteinnkallelser og svar, er standard tillatelsesinnstillinger, for eksempel Representant, kopier av **møterelaterte** meldinger som sendes til meg, tilstrekkelig. Du kan la **innbokstillatelsesinnstillingen** være på **Ingen**. Møteinnkallelser og svar går direkte til representantens innboks.

    > [!NOTE]
    > Som standard får representanten **redigeringstillatelse (kan lese, opprette og endre elementer)** til **Kalender-mappen.** Når representanten svarer på et møte på dine vegne, legges den automatisk til i **Kalender-mappen.**

5. Hvis du vil sende en melding for å varsle representanten om de endrede tillatelsene, merker du av for Send automatisk en melding til representant som **oppsummerer disse tillatelsene.**
6. Hvis du vil, merker du av **for Representanten kan se mine private elementer.**

    > [!IMPORTANT]
    > Denne innstillingen påvirker alle Exchange mapper. Dette omfatter alle mappene E-post, Kontakter, Kalender, Oppgaver, Notater og Logg. Det er ikke mulig å gi tilgang til private elementer i bare angitte mapper.

7. Velg **OK**.

    > [!NOTE]
    >
    > - Meldinger som sendes med send på vegne av-tillatelsene, omfatter både representantens og navnene dine ved siden av **Fra**. Når en melding sendes med Send som-tillatelser, vises bare navnet ditt.
    > - Når du har lagt til noen som representant, kan de legge Exchange postboksen til vedkommendes Outlook profil. Hvis du vil ha instruksjoner, kan du se Administrere en [annen persons e-post- og kalenderelementer](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Slik fjerner du en representant Outlook for Windows:

1. Klikk på **Fil-fanen.**
2. Klikk på **Konto-Innstillinger** etterfulgt av **Representanttilgang**.
3. Velg navnet på representanten du vil endre tillatelser for, og klikk deretter Fjern **etterfulgt** av **OK**.

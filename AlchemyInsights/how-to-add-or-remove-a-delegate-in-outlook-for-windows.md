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
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573576"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Slik legger du til eller fjerner en representant i Outlook for Windows

Slik legger du til en representant i Outlook for Windows: 

1. Klikk **fil** -fanen etterfulgt av **konto innstillinger**, og velg deretter **representant tilgang**.
2. Klikk på **Legg til**. Hvis **Legg til** ikke vises, kan det være at en aktiv tilkobling ikke finnes mellom Outlook og Exchange. Status linjen i Outlook viser tilkoblings statusen.
3. Skriv inn navnet på personen du vil angi som representant, eller søk og velg navnet i søke resultat listen.

    > [!NOTE]
    > Representanten må være en person i organisasjonens globale adresse liste (GAL).
4. Klikk **Legg til** etterfulgt av **OK**.
5. Godta standard innstillingene for tillatelser i dialog boksen **representant tillatelser** , eller velg egen definerte tilgangs nivåer for Exchange-mapper.

    - Hvis en representant bare trenger tillatelse til å arbeide med møte innkallelser og svar, er standard tillatelses innstillinger som **representant mottar kopier av møte relaterte meldinger som sendes til meg** , er tilstrekkelig. Du kan la innstillingen for tillatelse til **innboksen** bli **værende.** Møte invitasjoner og svar vil gå direkte til representantens innboks.

    > [!NOTE]
    > Som standard er representanten gitt **redaktør (kan lese, opprette og endre elementer)** tillatelse til **Kalender** -mappen. Når representanten svarer på et møte på vegne av deg, legges det automatisk til i **Kalender** -mappen.

5. Hvis du vil sende en melding for å varsle representanten om de endrede tillatelsene, merker du av for **Send automatisk melding til representant oppsummering av disse tillatelsene** .
6. Hvis du vil, merker du av for **Representanten kan se mine private elementer** .

    > [!IMPORTANT]
    > Denne innstillingen påvirker alle Exchange-mapper. Dette inkluderer alle mapper for e-post, kontakter, kalender, oppgaver, notater og logg. Det er ikke mulig å gi tilgang til private elementer i bare bestemte mapper.

7. Velg **OK**.

    > [!NOTE]
    >
    > - Meldinger som sendes med Send på vegne av-tillatelser, omfatter både representantens og navnene ditt ved siden av **fra**. Når en melding sendes med Send som-tillatelser, vises bare navnet ditt.
    > - Når du har lagt til en representant, kan de legge til Exchange-postboksen i Outlook-profilen sin. Hvis du vil ha instruksjoner, kan du se [administrere en annen persons e-post og kalender elementer](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Slik fjerner du en representant i Outlook for Windows:

1. Klikk på **fil** -fanen.
2. Klikk på **konto innstillinger** etterfulgt av **representant tilgang**.
3. Velg navnet på representanten du vil endre tillatelser for, og klikk deretter på **Fjern** etterfulgt av **OK**.

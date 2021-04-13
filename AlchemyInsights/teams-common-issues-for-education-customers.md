---
title: Teams vanlige problemer for Education-kunder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 893c8cacaf089932014ba7a3ea6122d17da38cdd
ms.sourcegitcommit: ef7ec42aba3c06aa8966dfac71cec18c08e7acf8
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2021
ms.locfileid: "51692403"
---
# <a name="teams-common-issues-for-education-customers"></a>Teams vanlige problemer for Education-kunder

**For Education-kunder:**

Hvis du trenger hjelp til å distribuere Teams til bruk i fjernundervisning, kan du besøke [FastTrack Center](https://www.microsoft.com/fasttrack) for å sende inn en forespørsel. Se følgende vanlige problemer for Teams Education-kunder:

- Ser du meldingen «**Du går glipp av ting!**»? kan du se [Aktivere Microsoft Teams for skolen](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). I EDU-tenanter er ikke Microsoft Teams aktivert som standard, du må slå den på først.

- **Ny på Teams?** Se gjennom [Ekstern undervisning og læring i Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) for å se den mest oppdaterte veiledningen om hvordan du konfigurerer skolen din, timeplanleggingen, virtuelle møter og deler innhold med elever.

- Når du har aktivert dette, kan brukerne kjøre Teams, enten ved å installere [stasjonære](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) og [mobile klienter](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients), eller fra nettleseren på https://teams.microsoft.com.

- **Aktivere gjestetilgang i Teams**: Gå gjennom [sjekkliste for gjestetilgang i Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist), og kontroller at alle trinnene er fullført.
    - [Slik fungerer gjestetilgang i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Oppsett – sjekkliste for gjestetilgang i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Slik blir en gjest med i et team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-møter og innringing**: Trenger du hjelp til å slå på eller konfigurere telefonkonferanse i Microsoft Teams? Er denne brukeren nylig opprettet? Hvis dette er tilfelle, må du vente i 2–24 timer før innstillingene trer i kraft. Hvis du vil kontrollere at brukeren er lisensiert for telefonkonferanse og har et vanlig nummer:
    1. Gå til «Aktive brukere», og velg den aktuelle brukeren.
    2. Velg enten **Lisenser og apper** eller klikk på **Rediger** på **Produktlisenser** avhengig av versjonen av administrasjonssenteret.
    3. Kontroller at brukeren har valgt lisenser for Telefonkonferanse, Microsoft Teams og Skype for Business Online (plan 2).
    4. Klikk på **Vis alle** og deretter **Teams** i Administrasjonssentre for bruker.
    5. Klikk på **Eldre portal** i Administrasjonssenter for Microsoft Teams.
    6. Klikk på **Telefonkonferanse** og deretter **Brukere** i Administrasjonssenter for Skype for Business.
    7. Velg den aktuelle brukeren, og kontroller at brukeren har et standard nummer.

    Hvis du vil ha mer informasjon, kan du se [Microsoft Teams samtaleplaner](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) eller ringe Microsoft Commerce fakturaavdeling for å få hjelp med lisensieringsrelaterte spørsmål.

    Flere ressurser

    - [Møter og konferanser i Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Lydkonferanser](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Møtepolicyer**: Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere, for møter som er planlagt av brukere i organisasjonen. Når du har opprettet en policy og gjort ønskede endringer, kan du tilordne brukere til policyen.

    - **Endre eller opprette en møtepolicy**: For å endre eller opprette en møtepolicy, går du til **Administrasjonssenter for Microsoft Teams > Møter > Møtepolicyer**. Velg en policy fra listen, eller tryk på **Legg til**. Hvis du oppretter en ny policy, legger du til navn og beskrivelse. Navnet kan ikke inneholde spesialtegn eller være lenger enn 64 tegn. Velg innstillinger, og klikk deretter på **Lagre**. 
    
        La oss for eksempel si at du har flere brukere, og du ønsker å begrense båndbredden møtet deres krever. Opprett en ny egendefinert policy som heter «Begrenset båndbredde», og deaktiver disse innstillingene:

        Under **Lyd og video**:
        - Slå av **Tillat at opptak lastet opp til skyen**.
        - Slå av **Tillat IP-video**.

        Under **Deling av innhold**:

        - Deaktiver skjermdelingsmodus.
        - Slå av **Tillat tavle**.
        - Slå av **Tillat delte notater**.

        Deretter **tilordner du policyen til brukerne**:

    1. Gå til **Brukere**, og klikk deretter på brukeren i navigasjonsruten til venstre i Administrasjonssenter for Microsoft Teams.
    2. Velg brukeren ved å klikke til venstre for brukernavnet og deretter klikke på **Redigere innstillinger**.
    3. Velg policyen du vil tilordne, og klikk deretter på **Bruk**, under **Møtepolicy**.

    Hvis du vil tilordne flere brukere samtidig, kan du se [Redigere flere Teams-brukerinnstillinger samtidig](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Du kan også gjøre dette:
    1. Gå til **Møter > Møtepolicyer** i navigasjonsruten til venstre i Administrasjonssenter for Microsoft Teams.
    2. Velg policyen ved å klikke til venstre for policynavnet.
    3. Klikk på **Behandle brukere**.
    4. Søk etter bruker etter visningsnavn eller brukernavn, velg navnet og klikk deretter på **Legg til**, i **Administrere brukere**-fanen. Gjenta dette trinnet for hver figur du vil legge til.
    5. Når du er ferdig med å legge til brukere, klikker du på **Lagre**.

- **Feilsøke manglende numerisk tastatur**:
    - Kontroller at brukeren har en [Teams-lisens](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Kontroller at brukeren har et tilordnet [abonnement](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Aktiver brukerne for [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Feilsøke Teams-pålogging**: Først kontrollerer du at [Microsoft Teams-tjenesten er god](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Se etter eventuelle vanlige feilkoder og se gjennom [Hvorfor har jeg problemer med å logge på Microsoft Teams](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)? Det kan også hende at du må gå gjennom [Identitetsmodeller og godkjenning i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

---
title: Teams-temaet catchall
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: e1d5f07a10fc014ac8b983bd6dd426c13fc7b807
ms.sourcegitcommit: 7d787b8c5af223e2711b4c2a2ca55ce2bdc25aea
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2020
ms.locfileid: "42856476"
---
# <a name="teams-common-issues-and-resolutions"></a>Kjente problemer og løsninger for Teams

Hvis du vil ha et mer nøyaktig svar, kan du prøve å omformulere spørsmålet til å inkludere feil som du ser, eller Teams-funksjoner du bruker.

Hvis du trenger hjelp til å distribuere Teams for å støtte eksterne arbeidere på grunn av COVID-19, kan du se [Støtte eksterne arbeidere som bruker Microsoft Teams](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams). Det kan også hende at du er kvalifisert for distribusjonshjelp fra Microsoft 365 FastTrack-programmet. Gå til [FastTrack Center](https://www.microsoft.com/fasttrack) for å sende inn en forespørsel.

For alle Teams-kunder:

- **Ny på Teams?** Se [Komme i gang med Microsoft Teams](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start).
- **Aktivere gjestetilgang i Teams:** Gå gjennom [sjekkliste for gjestetilgang i Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist), og kontroller at alle trinnene er fullført. Flere ressurser:
    - [Slik fungerer gjestetilgang i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Oppsett – sjekkliste for gjestetilgang i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Slik blir en gjest med i et team](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-møter og innringing**: Trenger du hjelp til å slå på eller konfigurere telefonkonferanse i Microsoft Teams? Er denne brukeren nylig opprettet? Hvis dette er tilfelle, må du vente i 2–24 timer **før innstillingene trer i kraft**. 

    Slik kontrollerer du at brukeren er lisensiert for telefonkonferanse og har et standard nummer:
    1.    Gå til Aktive brukere, og velg den aktuelle brukeren.
    2.    Velg enten **Lisenser og apper** eller klikk på **Rediger** på **Produktlisenser** avhengig av versjonen av administrasjonssenteret.
    3.    Kontroller at brukeren har valgt lisenser for Telefonkonferanse, Microsoft Teams og Skype for Business Online (plan 2).
    4.    Klikk på **Vis alle** og deretter **Teams** i Administrasjonssentre for bruker.
    5.    Klikk på **Eldre portal** i Administrasjonssenter for Microsoft Teams.
    6.    Klikk på **Telefonkonferanse** og deretter **Brukere** i Administrasjonssenter for Skype for Business.
    7.    Velg den aktuelle brukeren, og kontroller at brukeren har et standard nummer.
    
    Hvis du vil ha mer informasjon, kan du se [Abonnementer i Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) eller ringe fakturaavdelingen for Microsoft Commerce for hjelp med lisensieringsrelaterte spørsmål.

    Flere ressurser:

    - [Møter og konferanser i Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Telefonkonferanser i Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Teams Exploratory-lisens**: Med Microsoft Teams Exploratory-opplevelsen kan brukere i organisasjonen som har Azure Active Directory (AAD) og ikke er lisensierte for Teams, starte en utforskende opplevelse av Teams. Administratorer kan slå denne funksjonen av eller på for brukere i organisasjonen. Den tidligere [prøveversjonen av kommersiell Microsoft-sky](https://docs.microsoft.com/microsoftteams/iw-trial-teams) er nå erstattet av Teams Exploratory-opplevelsen.

    Flere ressurser:

    - [Slik registrerer brukere seg for Teams Exporatory-opplevelsen](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience)
    - [Administrere Teams Exploratory-opplevelsen](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience)

- **Private kanaler**: Private kanaler i Microsoft Teams oppretter fokuserte områder for samarbeid i teamene. Bare brukere på teamet som er eiere eller medlemmer av den private kanalen, har tilgang til kanalen. Alle, inkludert gjester, kan legges til som medlem i en privat kanal, så lenge de allerede er medlemmer av teamet.

    Du bør bruke en privat kanal hvis du vil begrense samarbeidet til de som har behov for å vite, eller hvis du vil fremme kommunikasjonen mellom en gruppe personer som er tilordnet til et bestemt prosjekt, uten å måtte opprette et ekstra team å administrere.

    Flere ressurser:
    - [Privat kanaloppretting og medlemskap](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership)
    - [Administrere private kanalmedlemskap og innstillinger](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings)

- **Møtepolicyer**: Møtepolicyer brukes til å kontrollere funksjonene som er tilgjengelige for møtedeltakere for møter som er planlagt av brukere i organisasjonen. Når du har opprettet en policy og gjort ønskede endringer, kan du tilordne brukere til policyen. 
    - **Endre eller opprette en møtepolicy**: For å endre eller opprette en møtepolicy, går du til **Administrasjonssenter for Microsoft Teams > Møter > Møtepolicyer**. Velg en policy fra listen, eller velg Legg til. Hvis du oppretter en ny policy, legger du til navn og beskrivelse. Navnet kan ikke inneholde spesialtegn eller være lenger enn 64 tegn. Velg innstillinger, og klikk deretter på **Lagre**.

        La oss for eksempel si at du har flere brukere, og du ønsker å begrense hvor mye båndbredde møtet deres krever. Opprett en ny egendefinert policy som heter «Begrenset båndbredde», og deaktiver disse innstillingene:

        Under **Lyd og video**:
        - Slå av Tillat at opptak lastet opp til skyen.
        - Slå av Tillat IP-video.

        Under **Deling av innhold**:
        - Deaktiver skjermdelingsmodus.
        - Slå av Tillat tavle.
        - Slå av Tillat delte notater.

        Deretter tilordner du policyen til brukerne.

- **Tilordne en møtepolicy til brukere**

    1. Gå til **Brukere**, og klikk deretter på brukeren i navigasjonsruten til venstre i Administrasjonssenter for Microsoft Teams.
    2. Velg brukeren ved å klikke til venstre for brukernavnet og deretter klikke på **Redigere innstillinger**.
    3. Velg policyen du vil tilordne, og klikk deretter på **Bruk**, under **Møtepolicy**.

    Hvis du vil tilordne flere brukere samtidig, kan du se [Redigere flere Teams-brukerinnstillinger samtidig](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk). Du kan også gjøre dette:

    1. Gå til **Møter > Møtepolicyer** i navigasjonsruten til venstre i Administrasjonssenter for Microsoft Teams.
    2. Velg policyen ved å klikke til venstre for policynavnet.
    3. Velg **Administrere brukere**.
    4. Søk etter bruker etter visningsnavn eller brukernavn, velg navnet og klikk deretter på **Legg til**, i **Administrere brukere**-fanen. Gjenta dette trinnet for hver figur du vil legge til.
    5. Når du er ferdig med å legge til brukere, klikker du på **Lagre**.

- **Feilsøke manglende numerisk tastatur:**  

    - Kontroller at brukeren har en [Teams-lisens](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Kontroller at brukeren har et tilordnet [abonnement](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Aktiver brukerne for [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Feilsøke Teams-pålogging:** Først kontrollerer du at [Microsoft Teams-tjenesten er god](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Se etter eventuelle vanlige feilkoder og se gjennom [Hvorfor har jeg problemer med å logge på Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)  Det kan også hende at du må gå gjennom [Identitetsmodeller og godkjenning i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

**For Education-kunder:**

Hvis brukerne ser meldingen «Du går glipp av ting.» kan du se [Aktivere Microsoft Teams for skolen](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). I EDU-tenanter er ikke Microsoft Teams aktivert som standard, du må slå den på først.

Deretter ser du gjennom [Ekstern undervisning og læring i Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) for å se den mest oppdaterte veiledningen om hvordan du konfigurerer skolen din, timeplanleggingen, virtuelle møter og deler innhold med elever.

Til slutt må du sørge for at du sjekker ut opplæringsvideoer, lysbildefremvisninger og mye mer for IT-administratorer i Microsoft Teams her:https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training 

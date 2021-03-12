---
title: Feilsøke gruppeproblemer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714051"
---
# <a name="troubleshoot-group-issues"></a>Feilsøke gruppeproblemer

**Jeg trenger å tilordne en gruppe til en Azure AD-rolle**

Hvis du vil tilordne en Azure Active Directory-gruppe (AD) til en Azure AD-rolle, utfører du følgende trinn:

1. Opprette en ny gruppe – slik oppretter du en ny gruppe:

    a. Logg på administrasjonssenteret for Azure AD med privilegerte rolleadministrator- eller globale administratortillatelser. 
    b. Velg Azure Active Directory > grupper > alle grupper > Ny gruppe. 
    c. Opprett gruppen.

2. Tilordne rollen til gruppen under opprettelsen av gruppen eller etter at gruppen er opprettet.

    a. Hvis du vil tilordne en rolle til gruppen da gruppen ble opprettet, kan du aktivere veksleknappen for Azure AD-roller og opprette gruppen.
    b. Hvis du vil tilordne en rolle til gruppen etter at den er opprettet, går du til fanen Tilordnede roller for den nyopprettede gruppen og tilordner rollen til gruppen.

**Jeg må administrere medlemskap i en gruppe som er tilordnet Azure AD-rollen**

1. For å forhindre rettighetsutvidelse kan som standard bare privilegert rolleadministrator og global administrator endre medlemskapet til en gruppe som er tilordnet en rolle. De kan imidlertid velge å tilordne en eier for en slik gruppe, og delegere denne oppgaven. Hvis du vil ha mer informasjon, kan du se Bruke [skygrupper til å administrere rolletilordninger i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. For vanlige spørsmål og feilsøkingstips for å tilordne roller til grupper i Azure AD, kan du se [Feilsøkingsroller som er tilordnet til skygrupper.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dynamiske grupper**

1. Hvis du ikke finner de innebygde brukerattributtene, må du kontrollere at attributtet er i listen over støttede egenskaper.
2. Hvis du leter etter innebygde enhetsattributter, må du kontrollere at attributtet er i listen over enhetsattributter 
3. I tillegg til de innebygde bruker- og enhetsattributtene, kan du også bruke [utvidelsesattributter.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Når du har synkronisert utvidelsesattributter fra den lokale Windows Server AD eller fra et tilkoblet SaaS-program, skal attributtene være synlige i rullegardinlisten i regelverktøyet. Du finner det egendefinerte attributtnavnet i katalogen ved å spørre etter en brukers attributt ved hjelp av PowerShell og søke etter attributtnavnet. Disse kan også brukes når du konstruerer regler i regelsyntaksen.
4. Kontroller at leieren har riktig lisens. Dynamiske grupper krever at leieren har en Lisens for Azure AD P1 Premium. Du finner listen over Azure AD-lisensplaner [her.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security-lisensieringsplaner er tilgjengelig [her.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Kontroller at rollen til brukeren som oppretter den dynamiske gruppen, er global administrator, Intune-administrator, gruppeadministrator eller en brukeradministrator.
6. Gi gruppen tid til å fylle ut. Gruppen kan ta opptil 24 timer før den fyller ut for første gang eller etter at en regel endres, avhengig av størrelsen på tenanten.
7. Hvis du vil ha mer informasjon, kan du se [Opprette attributtbaserte regler for dynamisk gruppemedlemskap.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Jeg trenger å slette en gruppe**

1. Grupper kan slettes fra katalogen ved hjelp av Remove-AzureADGroup-cmdleten i Azure AD Powershell-modulen.
2. Før du prøver å slette en synkronisert gruppe i Azure AD, må du kontrollere at du har slettet alle tilordnede lisenser for å unngå feil.
3. Hvis du vil ha mer informasjon om å slette grupper, kan du [se Slette en gruppe med en tilordnet lisens.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Jeg trenger å gjenopprette en slettet gruppe**

1. Hvis en Office 365-gruppe slettes, kan den bare gjenopprettes opptil 30 dager før permanent sletting skjer. Når gruppen er slettet for godt, kan den ikke lenger gjenopprettes. Finn ut mer om hvordan du gjenoppretter [grupper her.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Denne funksjonaliteten støttes ikke for sikkerhetsgrupper og distribusjonsgrupper.
3. Sikre at du er autorisert til å gjenopprette en Office 365-gruppe. Globale administratorer, gruppeadministratorer, brukerkontoadministratorer, Intune-tjenesteadministratorer, partner tier1- eller tier2-støtte, og eieren av gruppen kan gjenopprette en gruppe.
4. Når en dynamisk gruppe slettes og gjenopprettes, vises den som en ny gruppe og fylles ut på nytt i henhold til regelen. Denne prosessen kan ta opptil 24 timer.
5. Hvis du vil ha mer informasjon om gjenoppretting av en slettet gruppe, kan du se Gjenopprette en slettet [Office 365-gruppe i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Konfigurasjon av policy for utløp av gruppe**

1. Denne funksjonaliteten støttes bare for Office 365-grupper, og ikke for sikkerhetsgrupper og distribusjonsgrupper.
2. Konfigurasjon og bruk av utløpspolicyen for Office 365-grupper krever en Azure AD Premium-lisens.
3. For øyeblikket kan bare én utløpspolicy konfigureres for Office 365-grupper på en leier.
4. Bare globale administratorer, gruppeadministratorer, brukeradministratorer og eieren av gruppen kan fornye en gruppe.
5. Hvis en Office 365-gruppe er utløpt, slettes den og kan bare gjenopprettes opptil 30 dager før permanent sletting skjer. Når gruppen er slettet for godt, kan den ikke lenger gjenopprettes. Finn ut mer om hvordan du gjenoppretter [grupper her.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Aktivitetsbasert automatisk fornyelse**

Brukeraktiviteter fra SharePoint, Outlook og Teams kan utløse automatisk fornyelse av grupper. Aktiviteter kontrolleres 35 dager før en gruppe utløper. Hvis det er aktivitet i løpet av den gjeldende livssyklusen for gruppen, fornyes gruppen automatisk, og e-postvarsel sendes ikke ut til gruppeeiere.

**Tidsberegning for utløpte grupper**

1. E-postvarsler sendes til Office 365-gruppeeiere 30 dager, 15 dager og 1 dag før gruppen utløper.
2. Når du konfigurerer utløpsdato for første gang, settes alle grupper som er eldre enn utløpsintervallet, til 35 dager frem til utløpsdato.
3. Utløpsdatoen for gruppen beregnes basert på gruppens fornyelsesdato, ikke basert på oppdateringsdatoen for policyen. Hvis utløpsdatoen oppdateres, endres ikke utløpsdatoen.
4. Hvis du vil ha mer informasjon, kan du se policy for utløp av [grupper](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) og fornyelse av e-postmeldinger og Gjenopprette en slettet [Office 365-gruppe i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Tillatelse til å opprette en gruppe**

Kontroller at du er autorisert til å opprette en ny gruppe. Globale administratorer kan deaktivere opprettelse av grupper i Azure-portalen eller tilgangspanelet. Det kan hende du trenger en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.

1. [Opprette en ny gruppe og legge til medlemmer i Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Opprette grupper i Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Deaktivere opprettelse av grupper i PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Administrere hvem som kan opprette grupper i Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Deaktivere velkomstvarselet for Office 365 via Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Administrative roller for Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Behandle opprettelsestillatelser for grupper**

1. Globale administratorer kan behandle opprettelsestillatelser for grupper for sikkerhet eller Office 365-grupper som er opprettet i Azure-portalen eller tilgangspanelet, ved å angi Brukere kan opprette sikkerhetsgrupper i **Azure-portaler,** eller brukere kan opprette **Office 365-grupper** i innstillingene for Azure-portalen i Alle grupper **> Generelt (Innstillinger)**.
2. Du kan også begrense opprettelse av grupper for å velge en gruppe med brukere hvis du har en Azure AD P1 Premium-lisens.

**Deaktivere velkomstvarsel for nye medlemmer i en Office 365-gruppe**

Velkomstvarselet som sendes til brukere som er lagt til i Office 365-grupper, kan deaktiveres ved å `UnifiedGroupWelcomeMessageEnabled` angi **False** i Powershell. Finn ut mer om denne [innstillingen her.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)














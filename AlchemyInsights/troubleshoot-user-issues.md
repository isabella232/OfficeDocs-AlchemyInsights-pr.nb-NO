---
title: Feilsøke bruker problemer
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901332"
---
# <a name="announcements"></a>Kunngjøringer

Følg veiledningen for Google for testing av kompatibilitet for å teste om appene er berørt. Google-veiledningen er tilgjengelig i https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Kontroller at du bruker System Web visning eller system leser når du logger på brukerne med Google-kontoer for forbrukere. Hvis du vil ha mer informasjon, kan du se problemer med å [logge deg på programmet (ene) ved hjelp av Chrome-leser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Jeg kan ikke opprette en ny bruker i Azure AD-katalogen**

Hvis du vil feilsøke problemet med at du ikke kan opprette en ny bruker i Azure AD, utfører du følgende trinn:

1. Kontroller at du har tillatelse til å opprette en ny standard bruker. Bare rollen global administrator eller bruker administrator i Azure Active Directory (AD) kan opprette en ny standard bruker. Hvis du ikke er i en av disse rollene, ber du administratoren om å legge deg til en av disse rollene, eller for å opprette den nye bruker kontoen for deg.
2. Kontroller at bruker navnet er i et domene som er bekreftet i Azure AD. Hvis du ikke har bekreftet egen definerte domene navn i Azure AD, kan du bruke det første Azure AD-domenet, som slutter med *. onmicrosoft.com.
3. Kontroller at bruker navnet er i et domene som ikke er i forbund for Azure AD, fra din lokale annonse. Brukere kan ikke legges til i skyen med domene navn som er forbundet fra lokal.
4. Kontroller at ingen andre brukere eller kontakter allerede har bruker navnet du vil tilordne til den nye brukeren. Bruker navn må være unike på tvers av Azure AD.
5. Se [Azure ad Roles og administratorer](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for Azure ad.
6. Se [domene navnene](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) for Azure ad.
7. Se gjennom [overvåkings logger](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) for å se mer detaljert informasjon om en nylig opprettet eller slettet bruker, for eksempel hvem som utførte handlingen og når.
8. Hvis du vil ha mer informasjon om hvordan du legger til nye brukere, kan du se [bruke Azure-portalen til å opprette en ny bruker i Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Hvis du vil ha mer informasjon om administrator rolle tillatelser i Azure AD, kan du se [Azure ad administrative roller](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Hvis du vil ha mer informasjon om hvordan du oppretter en bruker med Azure AD PowerShell, kan du se [Azure ad PowerShell for å opprette en ny bruker](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem med registrering av selv betjening**

Hvis du vil feilsøke problemer med registrering av selv betjening, utfører du følgende trinn:

1. Hvis du vil bruke selv betjent registrering med programmene, må du først aktivere selv betjent registrering for leieren din. 
2. Hvis du vil aktivere et program for å støtte selv betjent registrering, kan du legge det til i bruker flyten. Neste gang du går til påloggings siden for dette programmet, ser du et alternativ **_ingen konto? Opprett en!_* _. Dette starter registrerings prosessen for selv betjening.
3. Hvis du vil ha informasjon om hvordan du bruker selv betjent registrering for å fylle ut en organisasjon i Azure AD, kan du se [selv betjent registrering for Azure ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Når du knytter bruker flyten til ett eller flere programmer, kan brukere som besøker appen, registrere seg og få en gjeste konto ved hjelp av alternativene som er konfigurert i bruker flyten. Hvis du vil ha mer informasjon om å registrere deg og få en gjeste konto, kan brukerne se [selv betjent registrering for gjeste brukere](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problem med å invitere en ekstern bruker**

Hvis du vil feilsøke problemer med å invitere en ekstern bruker, utfører du følgende trinn:

Pass på at du sender en bruker invitasjon til e-postadressen som Sams varer med navnet som brukeren logger på med. Hvis du sender invitasjonen til en brukers proxy-e-postadresse, kan ikke brukeren innløse den. Hvis du vil ha mer informasjon, kan du se [Azure ad B2B-dokumentasjonen](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Jeg kan ikke tilordne lisenser til en bruker**

Hvis du vil feilsøke problemer med å tilordne lisenser til en bruker, utfører du følgende trinn:

1. Hvis du vil administrere bruker lisenser, må du kontrollere at du bruker en konto med en av de nødvendige administrator rollene: Global administrator, lisens administrator eller bruker administrator. Du kan kontrollere brukerens rolle i kategorien **katalog rolle** på bruker blad.
2. Hvis du bruker Azure-portalen og tildeling av lisens mislykkes, klikker du varselet øverst til høyre. Dette åpner et blad med detaljer om hva som gikk galt. I de fleste tilfeller som er nok til å forstå og løse problemet.
3. Før en lisens kan tilordnes til en bruker, må du kontrollere at egenskapen **Bruk plassering** er angitt for brukeren. Kontroller at brukeren har denne egenskapen angitt ved å vise **profil** -fanen på bruker blad.
4. Kontroller at det er nok tilgjengelige lisenser for produktet du prøver å tilordne. Du kan se antallet tilgjengelige lisenser i Azure-portalen i [Azure Active Directory – > lisenser – > alle produkter](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Brukeren kan allerede ha en annen lisens for de tjenestene som er i konflikt med dem i den nye lisensen du prøver å tilordne. Hvis brukeren for eksempel har Exchange Online (plan 1)-tjenesten aktivert, kan du ikke tilordne en lisens med Exchange Online (plan 2). Deaktiver en av tjenestene for å tillate den nye lisens tilordningen. Hvis du bruker Azure-portalen eller PowerShell-cmdleter, viser **problem detaljer** -siden de spesifikke tjenestene som for år saker konflikten.
6. Hvis du prøver å fjerne en lisens og det mislykkes, kan brukeren ha andre lisenser med tjenester som er avhengige av tjenestene du prøver å fjerne. Hvis du bruker Azure-portalen eller PowerShell-cmdleter, viser feil meldingen de spesifikke tjenestene som har avhengigheter.
7. Hvis du vil forstå hvorfor en lisens ble lagt til/fjernet fra en bruker (for eksempel hvem andre i organisasjonen kan ha gjort endringer), må du kontrollere overvåkings loggene. Sett filteret til **lisens aktiviteter** for å vise alle endringer, inkludert skuespilleren som utførte dem.
8. Hvis du bruker Exchange Online, kan noen brukere i leieren være feil konfigurert med samme proxy-adresse. I slike tilfeller kan du se generelle feil meldinger når en lisens operasjon mislykkes. [Denne artikkelen](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) inneholder mer informasjon om dette problemet, inkludert informasjon om [hvordan du kobler til Exchange Online ved hjelp av ekstern PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Hvis du vil identifisere hvilke brukere i leieren, inneholder samme proxy-adresse, utfører du denne Exchange Online-cmdleten:

Køyrer

Get-Recipient | der {$ _. EmailAddresses – Sammenlign <user principal name> } | fL-navn, RecipientType, emailaddresses






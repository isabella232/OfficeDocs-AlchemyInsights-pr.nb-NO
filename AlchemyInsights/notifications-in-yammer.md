---
title: Varsler i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833588"
---
# <a name="notifications-in-yammer"></a>Varsler i Yammer

For å varsle deg om ny aktivitet i relevante samtaler, sender [Yammer deg varsler](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) enten via e-post eller – hvis du bruker Yammer på den mobile enheten – via push-varslinger. Som standard sender Yammer deg varsler for mange typer aktivitet i nettverket. Brukerne kan oppdatere e-postinnstillingene sine via Yammer-nettstedet, og push-varslinger konfigureres gjennom mobilappen. 

Yammer har lagt til støtte for [interaktive e-postmeldinger i Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Enkelte e-postmeldinger (kopier av meldinger) blir interaktive i Outlook på nettet. En fremtidig oppdatering vil hente dette til andre versjoner av Outlook.

**Typer varsler i Yammer**

- E-postmeldinger (oppdateringer fra en gruppe, noen inviterer deg til en-gruppe, mottar du en melding i innboksen og så videre).
- Push-varslinger (sendes til mobile enheter når du blir omtalt, mottar en melding i innboksen og så videre).
- Hurtigmenyer for skrivebordet (når du har installert skrivebordsversjonen av Yammer-appen, vil den vise såkalte «toast»-varsler for brukere.)
- Klokkevarsler (på selve Yammer-nettstedet vil brukerne se varsler for ulike hendelser. Det kan hende at disse varslene ikke alltid har et tilknyttet e-post- eller push-varsel.)

Mer [detaljert informasjon om varsler](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) er tilgjengelig.

**Behandle varsler**

Brukerne må behandle sine egne varsler. Informasjon er tilgjengelig på [hvordan du aktiverer og deaktiverer e-post- og mobiltelefon-varsler i Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Det er ikke mulig for administratorer å deaktivere alle varslinger eller kontrollere varsler, på vegne av brukerne. Administratorer kan [kontrollere logoen som er inkludert i e-postmeldinger, og om brukerne trenger å bekrefte meldinger](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) lagt ut via e-post.

**E-postmeldinger sendt til mange brukere i organisasjonen**

Noen ganger sendes en e-postmelding via e-post til Yammer, og den mottas av mange flere brukere i organisasjonen enn forventet. Dette skjer når en distribusjonsliste eller annen type ikke-individuell e-postadresser legges til i Yammer. Yammer fungerer ikke i alle tilfeller, enten en e-postadresse tilhører én enkelt bruker eller er en e-postadresse som fører til at én e-post blir levert til mange mottakere. Når dette problemet oppstår, må du utføre en handling for å [kansellere (deaktivere) den ugyldige brukeren med denne e-postadressen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) i Yammer. 

Hvis du vil redusere sjansen for at dette problemet oppstår, bør du:

1. [bruke Office 365-identitet](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) for Yammer-brukere
2. blokkere eksterne avsendere fra å sende e-post til organisasjonen, eller begrense avsendere til en godkjent liste

Hvis dette problemet oppstår, gjør du følgende:

1. Identifiser mottakeren av e-postmeldingen, som skal samsvare med brukeren i Yammer. All-in-sales@fabrikam.com er for eksempel en DL for alle selgere. Denne DL-en kan være identifiserbar fra Yammer-e-posten som mottas av brukere.
2. Bruk [deaktiver (hvilemodus) i Nettverksadmin](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) til å stoppe brukeren som har e-postadressen all-in-sales@fabrikam.com. Suspensjon kan angres, så det er tryggere enn sletting. Slettingen av brukeren vil skje automatisk etter 90 dager.
3. Hvis du vil, kan du se gjennom [Brukereksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) for å identifisere andre e-postadresser ikke tilknyttet brukere som skal suspenderes.

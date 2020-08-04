---
title: Bruk TeamViewer til å administrere Intune-enheter eksternt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555243"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Bruk TeamViewer til å administrere Intune-enheter eksternt

Enheter som administreres av Intune, kan administreres eksternt ved hjelp av [TeamViewer](https://www.teamviewer.com/).

Hvis du vil administrere Intune ved hjelp av TeamViewer, gjør du følgende: 

Begynn med å få legitimasjon fra TeamViewer til å konfigurere TeamViewer Connector på Intune. Dette gjør det mulig for administratoren å angi legitimasjon i Brukergrensesnittet for TeamViewer Connector under Enheter, en engangsoperasjon for å opprette koblingen mellom Intune og TeamViewer-tjenesten.

**Del 1: Starte en økt med en ekstern enhet**

1. Velg enheten du vil starte en ekstern økt med, under **Alle enheter.**
2. Fra **... Mer**velger du **Ny fjernhjelpsøkt**.
3. Velg **Ja** for å bekrefte at du vil opprette en ekstern økt.
    Når forespørselen "Starte en ny ekstern økt" er bekreftet av TeamViewer-tjenesten, ser du et alternativ for å **starte fjernhjelp** under detaljene i Oversikt (eller Essentials)-ruten for enheten. Velg **Se mer** for å utvide ruten og vise Fjernhjelp-statusen.
4. Velg **Start ekstern økt** for å starte økten på administratorsiden.
5. Velg å laste ned TeamViewer binære (Windows), og velg **Kjør**.<br/>
    **Merk at** Du kan ignorere alle nettlesersider som er åpnet for TeamViewer-nettstedet.

6. Bekreft forespørselen om at TeamViewer-appen skal gjøre endringer på enheten (bare Windows).
7. TeamViewer-appen starter og inkluderer øktkoden for å godkjenne tilkoblingen til den eksterne enheten.

**Del 2: På enheten som målrettes mot en ekstern økt**

1. Åpne Intune-firmaportalen.
2. Se etter et varselflagg: «IT-administratoren ber om kontroll over denne enheten for en ekstern assistanseøkt», og velg varselet.
3. Velg å laste ned TeamViewer-appen, eller erkjenn nedlasting av TeamViewer-appen fra appbutikken, og velg **Kjør**.
    **Merk at** Du kan ignorere alle nettlesersider som er åpnet for TeamViewer-nettstedet.

4. Bekreft forespørselen om at TeamViewer-appen skal gjøre endringer på enheten (bare Windows).
5. TeamViewer-appen starter og inkluderer øktkoden for å godkjenne tilkoblingen til den eksterne enheten.
6. En popup spør om du vil tillate økten å starte.

**Merk at** Øktkodene som genereres av TeamViewer-tjenesten, er bare engangsbruk. Hvis du mister tilkoblingen, må du:

1. Lukk forekomsten av TeamViewer-appen på den eksterne enheten og på administrasjonsarbeidsstasjonen.
2. Lukk firmaportalen på den eksterne enheten.
3. Start en ny "Ny fjernhjelp-økt" fra administrasjonsportalen.
4. Åpne firmaportalen på den eksterne enheten på nytt for å motta det nye varselet.
5. Last ned og åpne TeamViewer-appen på både den eksterne enheten og administrasjonsarbeidsstasjonen, som før.
---
title: Problem med attributt- og målfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481896"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem med attributt- og målfilter

**Problem med motstridende UPN-verdier**

Arbeidsdagen til AD-bruker klargjøring av arbeidsdagen til AD-bruker klargjøring viser feilmeldingen **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** Operasjonen mislyktes fordi UPN-verdien som er angitt for tillegg/endring, ikke er unik skogsdekkende. Feildetaljer: **CONSTRAINT_ATT_TYPE - userPrincipalName.**

**UserPrincipalName-verdien** som Workday-koblingen prøver å angi når du oppretter AD-brukerkontoen, finnes allerede i AD-måldomenet. Dette betyr at enten (1) brukeren allerede finnes og den samsvarende ID-kontrollen mislyktes for brukeren, eller (2) genererte UPN-genereringsregelen en motstridende verdi.

Her er de foreslåtte løsningstrinnene:

Hvis brukeren allerede finnes og den samsvarende ID-kontrollen ikke kunne koble arbeidsdagkontoen til Active Directory-kontoen, må du kontrollere om det samsvarende ID-attributtet (vanligvis **ansattID)** i både Arbeidsdag og AD har et nøyaktig samsvar. Hvis de ikke har noen treff, er det et dataproblem som må løses. Hvis for eksempel AnsattID i arbeidsdag er 001052 og i AD er det 1052, vil klargjøringsmotoren ikke koble de to kontoene og vil prøve å opprette en bruker som allerede finnes. Løsningen i dette tilfellet er å endre **AnsattID-verdien** i AD til å inkludere foranstilte nuller for å gjøre den til 001052.
Hvis det UPN-genererende uttrykket ikke genererer en unik verdi, kan du vurdere å bruke funksjonen **SelectUniqueValue** for dekopiering til å generere en unik verdi hver gang.

**Arbeidsdag til AD-klargjøring av bruker angir ikke noe lederattributtverdi for AD-brukerkonto**

Jobben for klargjøring av ad-bruker  for arbeidsdagen angir ikke lederens attributtverdi for AD-brukerkontoer. Det finnes to mulige scenarier når denne virkemåten vises:

1. Den overordnede i arbeidsdagen kan ikke løses til en tilsvarende AD-brukerkonto fordi den overordnede ikke er i omfanget.
2. I et **scenario med flere AD-domener** finnes ikke den overordnede i Workday i samme domene som brukeren.

Prøv disse trinnene for å løse problemet:

1. Hvis du har definert omfangsfiltre, må du først kontrollere om den overordnede er i omfang, og at den oppfyller omfangssetningen. Hvis den overordnede ikke oppfyller omfangsfilteret, endrer du filteret slik at den overordnede også beskjærer klargjøringsoperasjonen.
2. Hvis du har flere AD-domener, har koblingen en kjent begrensning av manglende evne til å løse referanser på tvers av domenebehandling.

Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)














---
title: Hvorfor er Legg til budsjett-knappen deaktivert for meg?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822644"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Hvorfor er Legg til budsjett-knappen deaktivert for meg?

Hvis du vil opprette et budsjett, trenger du én av følgende tillatelser:

- Administrasjonsgruppe, Abonnement, Ressursgruppeomfang
- Bidragsyter for kostnadsstyring
- Eier
- Bidragsyter
- Bare bedriftskunde: Registrering, avdeling, kontoomfang
- Registreringsadministrator (angi budsjett på registreringsomfang)
- Avdelingsadministrator (angi budsjett i avdelingsomfang)
- Kontoeier (angi budsjett i kontoomfang)
- Moderne kundeavtale: Faktureringskonto, faktureringsprofil, fakturadelomfang
- Azure-abonnementsoppretter

**Jeg opprettet et budsjett da kostnaden for gjeldende måned allerede var over budsjettert. Hvorfor mottok jeg ikke et varsel?**  
Hvis du allerede har overskredet en gitt kostnadsterskel når du oppretter et budsjett, vil ikke varselet bli utsende. Når en ny krets starter, hvis du bryter terskelen, vil varselet starte.

**Når bør jeg forvente å motta et varsel etter at jeg har overskredet en av mine definerte budsjettvarselsterskler?**  
Budsjetter evalueres hver 4. time. Det tar minst åtte timer før bruksdata når budsjettsystemet. På grunn av dette kan det ta så lang tid som 12 timer før varsler starter etter at du har overskredet en terskel.

**Hvorfor deaktiveres Startdato-knappen når jeg velger en periode for tilbakestilling av måned eller faktureringsmåned?**  
Budsjetter justeres etter gjeldende kalendermåned eller gjeldende faktureringsperiode (i tilfelle faktureringsmåned er valgt). Derfor forhåndsutmulerer vi denne verdien for deg.

**Hvorfor ser jeg ikke en graf over kostnadene mine i budsjettopprettingsopplevelsen?**  
Vi trenger minimum 2 måneder med kostnadsdata før vi kan gjengi en graf for å hjelpe deg med budsjettoppretting.

**Hvorfor kan jeg ikke angi et budsjett mot et abonnement jeg nettopp opprettet?**  
Når du har opprettet et abonnement, tar det 24–48 timer å behandle dataene før du setter et budsjett mot det.

**Budsjett-API-ressurser**

- [Budsjetter API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Gir operasjoner for å opprette og oppdatere budsjetter. Ved hjelp av Budsjetter-API-en kan du angi en budsjettterskel og konfigurere flere varsler til å starte når du nærmer deg denne terskelen. Varsler kan utløse en e-post eller en Azure-handlingsgruppe for å utføre automatisering. Merk: Filtrering for denne API-en justeres ikke etter spørrings-API-filtrering/-dimensjoner.
- [Budsjetter API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Opprett budsjetter med større funksjoner for kostnadsfiltrering enn v1. Filtreringen justeres etter kontrakten som brukes i API-ene for spørring og dimensjoner. Dette er den anbefalte budsjett-API-en for å bruke fremover.
- [Dimensjoner:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Gir operasjoner for å få støttede dimensjoner for bruk under en rekke omfang. Ved hjelp av Api for dimensjoner kan du hente en liste over dimensjoner som kan brukes som inndata for å generere spørringer med Spørrings-API-en.
- [Spørring:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Inneholder operasjoner for å få aggregerte kostnader og bruksdata basert på spørringen du angir. Ved hjelp av Spørrings-API-en kan du angi ønsket filtrering, sortering og gruppering etter alle tilgjengelige dimensjoner (som er tilgjengelig fra Api for dimensjoner).

**Prognoser for kostnader**

**Hvorfor ser jeg ikke prognoser for kostnadene mine i Kostnadsanalyse?**  
Det finnes flere årsaker til at prognoseprojeksjonen kan mangle for deg i Kostnadsanalyse, noen av dem er som følger:

1. Hvis kostnadsdataene er mindre enn 10 dager gamle, lastes ikke prognosediagrammet inn. Modellen krever minst 10 dager med nylige kostnadsdata for nøyaktige prognoser
2. Hvis du har valgt historiske datoer, vises ikke prognosediagrammet. Velg et datoområde med fremtidige datoer for at prognosediagrammet skal vises
3. Hvis kontoen har flere valutaer, vil prognosediagrammet bare vise kostnader for «Alle kostnader i USD»

**Hvorfor endres ikke prognosen når jeg gjør endringer i ressursene mine?**  
Prognosemodellen krever et par dager for å ta hensyn til endringer i kontoen og foretar ikke umiddelbare prognoser basert på endringer i ressurser  
For større trinn for økning eller reduksjon i ressurser, vil modellen ta litt lengre tid å justere til disse endringene for å ta hensyn til uregelmessigheter

**Hvorfor øker prognosen når jeg foretar en reservasjon eller et Marketplace-kjøp?**  
Prognosemodellen tar hensyn til faktiske kostnader og tar ikke hensyn til bruk og kjøp separat. For et engangskjøp vil modellen redusere anslagene etter 10 dager for å ta hensyn til den plutselige økningen i kostnader

**Jeg vil se prognoser for én enkelt dimensjon (f.eks. Meter)**  
Prognose støtter for øyeblikket totale kostnadsprojeksjoner og ikke for individuelle meter. Når «Gruppert etter» er en dimensjon, vil prognosene derfor være for totalsummen av alle elementene i dimensjonen

**Anbefalte dokumenter**

- [Hva er Azure Kostnadsstyring?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Anbefalte fremgangsmåter for Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysere kostnader og forbruk](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Utforske og analysere kostnader med kostnadsanalyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Kostnadsstyring: Priser](https://azure.microsoft.com/services/cost-management/#pricing)
- [Se gjennom kostnader i kostnadsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videoopplæring: Opprette et budsjett i Azure-portalen](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Forutsetninger for å vise og tilpasse budsjetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Opprette og administrere budsjetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurere automatisering med Azure Action Groups og Budgets API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Bruke kostnadsvarsler til å overvåke bruk og forbruk](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Anbefalte fremgangsmåter for kostnadsstyring](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Opplæringsvideoer**

- [Opprette et budsjett i Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrere kostnader med BUDSJETTER API og handlingsgrupper](https://go.microsoft.com/fwlink/?linkid=2147038)
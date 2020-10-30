---
title: Hvorfor er knappen Legg til budsjett deaktivert for meg?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807664"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Hvorfor er knappen Legg til budsjett deaktivert for meg?

Hvis du vil opprette et budsjett, trenger du en av følgende tillatelser:

- Administrasjons gruppe, abonnement, ressurs gruppe omfang
- Bidrags yter for kostnads administrasjon
- Bruker
- Wiki
- Bare Enterprise-kunde: registrering, avdeling, konto omfang
- Registrerings administrator (angi budsjett i registrerings området)
- Avdelings administrator (angi budsjett i avdelings omfang)
- Konto eier (angi budsjett ved konto omfang)
- Bare moderne kunde avtale: fakturerings konto, fakturerings profil, del omfang for fakturaer
- Azure-abonnement oppretter

**Jeg opprettet et budsjett da kostnadene for gjeldende måned allerede var over budsjettet. Hvorfor mottok jeg ikke et varsel?**  
Hvis du allerede har overskredet en angitt kostnads terskel når du oppretter et budsjett som varsel ikke vil starte. Når en ny syklus begynner, vil varselet aktiveres hvis du bryter terskelen.

**Når bør jeg forvente å motta et varsel etter at jeg har overskredet en av de definerte terskel verdiene for budsjett varsler?**  
Budsjetter evalueres hver 4. time. Det tar minst 8 timer før bruks data kommer til budsjett systemet. Hvis du har overskredet en terskel, kan det hende at varslene tar så lang som 12 timer å starte.

**Hvorfor er start dato-knappen deaktivert når jeg velger en periode for å null stille en måned eller fakturerings måned?**  
Budsjetter er justert til gjeldende kalender måned eller gjeldende fakturerings periode (i tilfelle fakturerings måned er valgt). Vi forhånd SUT fylte denne verdien for deg.

**Hvorfor ser jeg ikke et diagram over kostnadene i budsjett opprettelses opplevelsen?**  
Vi trenger minst to måneder med kostnads data før vi kan gjengi et diagram for å hjelpe deg med å opprette budsjett.

**Hvorfor kan jeg ikke angi et budsjett med et abonnement jeg nettopp opprettet?**  
Når du har opprettet et abonnement, tar dataene 24-48 timer å behandle før du angir et budsjett mot det.

**Budsjett API-ressurser**

- [BUDSJETTER API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): gir operasjoner til å opprette og oppdatere budsjetter. Ved hjelp av budsjett-APIEN kan du angi en budsjett terskel og konfigurere flere varsler som skal aktiveres når du nærmer seg denne grensen. Varsler kan utløse en e-post eller en Azure-handlings gruppe for å utføre automatisering. Obs! filtrering for denne APIEN er ikke justert med filtrering/dimensjoner for spørrings-API.
- [BUDSJETTER API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Opprett budsjetter med større kostnads filtrerings funksjoner enn v1. Filtrering justerer til kontrakten som brukes i API-er for spørring og dimensjoner. Dette er de anbefalte budsjett-APIEN for å flytte fremover.
- [Mål](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): gir operasjoner til å hente dimensjoner som støttes for bruk under en rekke ulike omfang. Ved hjelp av Dim ens IONS API kan du hente en liste over dimensjoner som kan brukes som inn data for å generere spørringer med spørrings-API-en.
- [Spørring](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): inneholder operasjoner for å hente aggregerte kostnader og bruks data basert på spørringen du angir. Ved hjelp av spørrings-API kan du angi ønsket filtrering, sortering og gruppering på alle tilgjengelige dimensjoner (som du får tilgang til fra dimensjons-APIEN).

**Prognoser for kostnader**

**Hvorfor ser jeg ikke prognoser for kostnadene mine i kostnads analyser?**  
Det finnes flere årsaker til hvorfor prognosen kan mangle for deg i kostnads analyser, som er noen av dem som følger:

1. Hvis kostnads dataene er mindre enn 10 dager gamle, vil ikke diagrammet lastes inn. Modellen krever minst 10 dager med nylige kostnads data for nøyaktige projeksjoner
2. Hvis du har valgt historiske datoer, vil ikke diagrammet være synlig. Velg et dato intervall med fremtidige datoer for diagrammet som skal vises
3. Hvis kontoen din har flere valutaer, vil prognosen bare beregne kostnader for alle kostnader i USD

**Hvorfor endres ikke prognosen når jeg gjør endringer i ressursene mine?**  
Prognosemodellen krever et par dager for å ta hensyn til endringer i kontoen, og gjør ikke umiddelbare prosjekter basert på endring i ressurser  
For større trinn ved å øke eller redusere i ressurser, tar det litt lengre tid å justere modellen for at disse endringene skal være i en uregelmessighet

**Hvorfor øker prognosen min etter at jeg har foretatt et reservasjons-eller Marketplace-kjøp?**  
Prognosemodellen anser de faktiske kostnadene og tar ikke hensyn til bruk og Kjøp separat. For et en gangs kjøp, vil modellen redusere projeksjonene etter 10 dager til konto for plutselig økning i kostnader

**Jeg vil se prognoser for en enkelt dimensjon (f.eks. Måling**  
Prognosen har for øyeblikket støtte for totale kostnads prosjekter og ikke for enkelt målere. Etter hvert som en dimensjon er gruppert etter, vil projeksjonene bli totalt for alle varene i dimensjonen

**Anbefalte dokumenter**

- [Hva er Azure kostnads behandling?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Anbefalte Fremgangs måter for Azure kostnads administrasjon](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analysere kostnader og utgifter](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Utforske og analysere kostnader med kostnads analyse](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Administrasjon av Azure-kostnad: pris setting](https://azure.microsoft.com/services/cost-management/#pricing)
- [Se gjennom kostnader i kostnads analyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video opplæring: opprette et budsjett i Azure-portalen](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Forutsetninger for å vise og tilpasse budsjetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Opprette og administrere budsjetter](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurere automatisering med Azure handlings grupper og budsjetter API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Bruke kostnads varsler til å overvåke bruk og forbruk](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gode Fremgangs måter for kostnads administrasjon](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Opplærings videoer**

- [Opprette et budsjett i Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Administrere kostnader med budsjetter-API og handlings grupper](https://go.microsoft.com/fwlink/?linkid=2147038)
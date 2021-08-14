---
title: Privileged Identity Management rolle
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973238"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM)-rolle

**Tillatelser gis ikke etter aktivering av en rolle**

Når du aktiverer en rolle i Azure AD Privileged Identity Management (PIM), overføres kanskje ikke aktiveringen umiddelbart til alle portaler som krever den privilegerte rollen. Noen ganger, selv om endringen overføres, kan nettbufring i en portal føre til at endringen ikke trer i kraft umiddelbart.

Hvis aktiveringen er forsinket, følger du disse trinnene:

1. Logg av Azure-portalen, og logg deretter på igjen. Når du aktiverer en Azure AD-rolle eller en Azure-ressursrolle, ser du trinnene i aktiveringen. Når alle trinnene er fullført, ser du koblingen Logg av. Du kan bruke denne koblingen til å logge av. Dette løser de fleste tilfeller for aktiveringsforsinkelse.
2. Kontroller at du er oppført som medlem av rollen i PIM.
3. Hvis du aktiverer administratorrollen Exchange, må du logge av og logge på igjen. Hvis problemet vedvarer, åpner du en støtteforespørsel og oppdrar dette som et problem. Hvis du bruker administratorrollen Exchange tilgang til sikkerhets- og samsvarssenteret, kan du se neste trinn.
4. Hvis du aktiverer en rolle for å få tilgang til sikkerhets- og samsvarssenteret, eller hvis du aktiverer SharePoint Administrator-rollen, vil du oppleve en viss aktiveringsforsinkelse fra noen minutter til noen timer. Dette er et kjent problem, og vi arbeider aktivt med disse teamene for å løse dette problemet så snart som mulig.

Hvis du vil ha mer informasjon, kan du se:

- [Aktivere Mine Azure AD-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivere mine Azure-ressursroller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Tillatelser fjernes ikke når du deaktiverer en rolle eller rolleaktiveringen utløper**

Når du deaktiverer en rolle i Azure AD Privileged Identity Management eller når en rolleaktiveringsperiode utløper, kan det være en forsinkelse der du fortsatt har tilgang.

Hvis deaktiveringen er forsinket, følger du disse trinnene:

1. Hvis du deaktiverer Exchange-administratorrollen eller rolleaktiveringsperioden utløper, og du ser en betydelig forsinkelse før tillatelsene fjernes, åpner du en støtteforespørsel og ber kundestøtteteknikeren om å hjelpe deg med å sende inn en billett med PAM-teamet (Privileged Access Management) i Office om dette problemet.
2. Hvis aktiveringsperioden er utløpt, men du fremdeles har nettleserøkten åpen, lukker du nettleseren. Du kan fortsette å bruke rollen til du lukker økten. Dette er et kjent problem, og vi ser på en mulig løsning for å aktivt tilbakekalle hver økt når aktiveringen er utløpt.

Hvis forsinkelsen er forskjellig fra disse to scenariene, kan du åpne en støtteforespørsel.

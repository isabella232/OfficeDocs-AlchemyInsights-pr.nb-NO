---
title: Rolle for privilegert identitets behandling
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088878"
---
# <a name="privileged-identity-managementpim-role"></a>PIM-rolle (Privileged Identity Management)

**Tillatelser gis ikke etter aktivering av en rolle**

Når du aktiverer en rolle i Azure AD Privileged Identity Management (PIM), kan det hende at aktiveringen ikke overføres direkte til alle portaler som krever rollen som privilegerte rettigheter. Noen ganger, selv om endringen er overført, kan Web buffer i en portal føre til at endringen trer i kraft umiddelbart.

Hvis aktiveringen er forsinket, følger du disse trinnene:

1. Logg av Azure-portalen, og logg deretter på igjen. Når du aktiverer en Azure AD-rolle eller en Azure-ressurs rolle, vil du se trinnene for aktiveringen. Når alle trinnene er fullført, vil du se koblingen Logg av. Du kan bruke denne koblingen til å logge av. Dette vil løse de fleste tilfeller for aktiverings forsinkelse.
2. Kontroller at du er oppført som medlem av rollen i PIM.
3. Hvis du aktiverer Exchange Administrator-rollen, må du passe på at du logger av og logger deg på igjen. Hvis problemet vedvarer, åpner du en støtte forespørsel og opphever dette som et problem. Hvis du bruker Exchange Administrator-rollen til å få tilgang til sikkerhets-og Samsvars senteret, kan du se neste trinn.
4. Hvis du aktiverer en rolle for å få tilgang til sikkerhets-og Samsvars senteret, eller hvis du aktiverer SharePoint-Administrator rollen, får du noen timer på opptil et par minutter. Dette er et kjent problem, og vi jobber aktivt med disse teamene for å løse dette problemet så snart som mulig.

Hvis du vil ha mer informasjon, kan du ta en titt på:

- [Aktivere mine Azure AD-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivere mine Azure-ressurser-roller i PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Tillatelser fjernes ikke etter at en rolle er deaktivert eller rolle aktiveringen utløper**

Når du deaktiverer en rolle i Azure AD Privileged Identity Management eller når en aktiverings periode for en rolle utløper, kan det oppstå en forsinkelse der du fortsatt har tilgang.

Hvis deaktivering er forsinket, følger du denne Fremgangs måten:

1. Hvis du deaktiverer Exchange Administrator-rollen eller aktiverings perioden for rolle utløper, og du legger merke til en betydelig forsinkelse før tillatelsene fjernes, kan du åpne en støtte forespørsel og be kunde støtte teknikeren om å hjelpe deg med å arkivere en billett med den privilegerte tilgangs behandlings gruppen (PAM) i Office om dette problemet.
2. Hvis aktiverings perioden er utløpt, men du fremdeles har åpnet nett leser økten, lukker du nett leseren. Du kan fortsette å bruke rollen til du lukker den økten. Dette er et kjent problem, og vi ser på en mulig løsning for aktivt å oppheve hver økt når aktiveringen er utløpt.

Hvis forsinkelsen er forskjellig fra disse to scenariene, kan du åpne en støtte forespørsel.

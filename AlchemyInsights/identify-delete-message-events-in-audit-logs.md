---
title: Identifisere slette meldings hendelser i overvåkings logger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696522"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåke logger for slettede e-postmeldinger

Microsoft slår på post boks overvåkings logging som standard i januar 2019. Hvis du vil se gjennom slette meldings hendelser for en bestemt bruker, må du aktivere slette handlingene for overvåking manuelt. Hvis overvåkings logging for post boks allerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du Fremgangs måten nedenfor.

1. Logg på [sikkerhets & samsvars senter for Microsoft 365](https://protection.office.com/)

2. Klikk **Søk og undersøkelser** , og velg **Søk i overvåkings Logg**.

3. Velg dato området i feltene **Start dato** og **slutt dato** . Angi bruker navnet for brukeren du vil undersøke (brukeren som slettet elementene). I **aktiviteter** -feltet velger du **slettede meldinger fra Slettede elementer-mappen** og **flyttede meldinger til Slettede elementer-mappen**.

4. Klikk **Søk**.

Velg en overvåkings post i resultatene. Klikk **mer informasjon**i under menyen detaljer. Tilleggs informasjon om det slettede elementet (for eksempel Emne linjen og plasseringen av elementet når det er slettet) vises i **AffectedItems** -feltet. **ClientInfoString** -egenskapen vises hvis slettingen ble utført i Outlook, Outlook på nettet (tidligere kjent som Outlook Web App) eller en annen enhet.

Hvis du vil ha mer informasjon, kan du se [finne ut hvem som konfigurerte videre sendingen av e-post](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Obs!** du kan ikke hente slettede elementer ved hjelp av funksjonen for overvåkings logg. Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).

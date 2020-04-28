---
title: Legge til eksterne brukere i en distribusjonsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910941"
---
# <a name="add-external-users-to-a-distribution-group"></a>Legge til eksterne brukere i en distribusjonsgruppe

Legge til en ekstern kontakt i en distribusjonsgruppe (DG) er en to-trinns prosess:
  
1. Opprett en e-postkontakt for den eksterne brukeren:
    
    1. Gå til **Brukere** > [kontakter-siden](https://admin.microsoft.com/adminportal/home#/Contact) i administrasjonssenteret. 
    
    2. Velg **Legg til en kontakt**.
    
    3. Skriv inn informasjonen for kontakten, og velg **Legg til**.
    
2. Legg til e-postkontakten i DG:
    
    1. Gå til > [Gruppergrupper-siden](https://admin.microsoft.com/adminportal/home#/groups) i administrasjonssenteret. **Groups** 
    
    2. Finn DG du vil legge til den eksterne brukeren i, og velg den for å åpne redigeringsdialogboksen.
    
    3. Velg Vis alle på **Medlemmer-fanen,** **og administrer medlemmer**. 
    
    4. Velg **Legg til medlemmer**.
    
    5. Velg e-postkontakten du opprettet i forrige trinn, og velg deretter **Lagre**.
    
Hvis de eksterne brukerne ikke kan sende e-post til DG eller ikke motta e-post fra den etter å ha fulgt disse trinnene, kan ikke sende e-post til DG eller ikke motta e-post fra den, men det kan være at DG er merket for å bare tillate e-post fra interne brukere. Du kan sjekke denne konfigurasjonen og fikse den ved å følge instruksjonene [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Merk:** Disse instruksjonene gjelder ikke hvis gruppens type er "Microsoft 365-gruppe" i stedet for "Distribusjonsgruppe". Hvis det er tilfelle, kan du legge til den eksterne brukeren direkte i gruppen fra Outlook. Detaljert informasjon om Microsoft 365 Grupper gjester samt instruksjoner for å legge til eksterne gjester kan bli funnet i [denne artikkelen](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  
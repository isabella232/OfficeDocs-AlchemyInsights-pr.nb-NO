---
title: Legge til eksterne brukere i en distribusjonsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934842"
---
# <a name="add-external-users-to-a-distribution-group"></a>Legge til eksterne brukere i en distribusjonsgruppe

Å legge til en ekstern kontakt i en distribusjonsgruppe (DG) er en totrinns prosess:
  
1. Opprette en e-postkontakt for den eksterne brukeren:
    
    1. Gå til Brukere-kontakter-siden i **administrasjonssenteret.**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Velg **Legg til en kontakt**.
    
    3. Skriv inn informasjonen for kontakten, og velg **Legg til**.
    
2. Legg til e-postkontakten i DG:
    
    1. Gå til Grupper grupper-siden i   >  [](https://admin.microsoft.com/adminportal/home#/groups) administrasjonssenteret. 
    
    2. Finn DG-en du vil legge til den eksterne brukeren i, og velg den for å åpne redigeringsdialogboksen.
    
    3. Velg Vis **alle** og behandle medlemmer på **Medlemmer-fanen.** 
    
    4. Velg **Legg til medlemmer**.
    
    5. Velg e-postkontakten du opprettet i forrige trinn, og velg deretter **Lagre**.
    
Hvis de eksterne brukerne ikke kan sende e-postmeldinger til DG eller ikke motta e-postmeldinger fra det etter å ha fulgt disse trinnene, kan det være at DG er merket for bare å tillate e-postmeldinger fra interne brukere. Du kan kontrollere denne konfigurasjonen og løse problemet ved å følge instruksjonene [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Obs!** Disse instruksjonene gjelder ikke hvis gruppens type er «Microsoft 365 gruppe» i stedet for «Distribusjonsgruppe». Hvis dette er tilfellet, kan du legge til den eksterne brukeren direkte i gruppen fra Outlook. Detaljert informasjon om Microsoft 365 Grupper-gjester samt instruksjoner for å legge til eksterne gjester finner du i [denne artikkelen.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  
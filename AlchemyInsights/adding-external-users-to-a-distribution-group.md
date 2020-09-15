---
title: Legge til eksterne brukere i en distribusjons gruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663522"
---
# <a name="add-external-users-to-a-distribution-group"></a>Legge til eksterne brukere i en distribusjons gruppe

Å legge til en ekstern kontakt i en distribusjons gruppe (DG) er en to trinns prosess:
  
1. Opprette en e-postkontakt for den eksterne brukeren:
    
    1. Gå til **brukerens**  >  [kontakter](https://admin.microsoft.com/adminportal/home#/Contact) -side i administrasjons senteret. 
    
    2. Velg **Legg til en kontakt**.
    
    3. Skriv inn informasjonen for kontakten, og velg **Legg til**.
    
2. Legg til e-postkontakten i DG:
    
    1. Gå til **grupper**  >  [grupper](https://admin.microsoft.com/adminportal/home#/groups) -siden i administrasjons senteret. 
    
    2. Finn DG du vil legge til den eksterne brukeren i, og velg den for å åpne dialog boksen Rediger.
    
    3. Velg **Vis alle og behandle medlemmer**på fanen **medlemmer** . 
    
    4. Velg **Legg til medlemmer**.
    
    5. Velg e-postkontakten du opprettet i forrige trinn, og velg deretter **Lagre**.
    
Hvis de eksterne brukerne ikke kan sende e-postmeldinger til DG eller ikke motta e-postmeldinger fra det, kan det være at DG er merket for bare å tillate e-postmeldinger fra interne brukere. Du kan kontrollere denne konfigurasjonen og rette den ved å følge instruksjonene [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Obs!** Disse instruksjonene gjelder ikke hvis gruppens type er Microsoft 365 Group i stedet for "distribusjons gruppe". Hvis det er tilfelle, kan du legge til den eksterne brukeren direkte i gruppen fra Outlook. Detaljert informasjon om Microsoft 365 grupper gjester samt instruksjoner for hvordan du legger til eksterne gjester, finner du i [denne artikkelen](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  
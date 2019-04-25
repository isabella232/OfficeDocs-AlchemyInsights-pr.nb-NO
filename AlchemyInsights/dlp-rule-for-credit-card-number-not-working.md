---
title: DLP-regel for kredittkortnummer fungerer ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404521"
---
Har du problemer med **Data tap forebygging (DLP)** fungerer ikke for innhold som inneholder et **Kredittkortnummer** når du bruker en type for DLP sensitiv informasjon i O365? I så fall må du kontrollere innholdet inneholder nødvendig informasjon til å utløse den DLP-policyen når de evalueres. For eksempel et **kredittkort policy** konfigurert med en konfidenskoeffisienten for 85%, for følgende evalueres og må registreres for at regelen skal utløse: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 sifre, noe som kan være formatert eller uformatert (dddddddddddddddd) og må bestå testen Luhn. 
    
- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Svært komplekse og robust mønster som oppdager kort fra alle store merker over hele verden, inkludert Visa, Mastercard, oppdage kort, JCB, American Express, gavekort og diner-kort. 
    
- **[Kontrollsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrollsum 
    
- **[Definisjon:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP-policy er 85% sikker på at det har oppdaget at sensitive opplysninger hvis, i en avstand på 300 tegn: 
    
  - Til Func_credit_card å finne innhold som samsvarer med mønsteret.
    
  - Ett av følgende er sant: 
    
  - Det finnes et nøkkelord fra Keyword_cc_verification.
    
  - Du finner et nøkkelord fra Keyword_cc_name
    
  - Funksjonen Func_expiration_date søker etter en dato i formatet riktig dato.
    
  - Kontrollsummen sender
    
    Hvis du for eksempel vil følgende eksempel utløse for en Policy for DLP kredittkort nummer:
    
  - Visa: 4485 3647 3952 7352 
    
  - Utløper: 2/2009
    
Hvis du vil ha mer informasjon om hva som trengs for et **Kredittkortnummer** kan oppdages for innholdet, kan du se delen nedenfor i denne artikkelen: [Hva the Sensitive informasjonstyper se etter kredittkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Å bruke en annen innebygd sensitiv informasjon, se følgende artikkel for å få informasjon på det som er nødvendig for andre typer: [se hva den Sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  


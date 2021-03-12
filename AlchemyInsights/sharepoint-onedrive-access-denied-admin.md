---
title: Feilsøk meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707963"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøke meldinger ingen tilgang i administrasjonssenteret for SharePoint/OneDrive

Hvis du får melding om at tilgangen er avvist når du prøver å gå til administrasjonssenteret for Sharepoint/OneDrive, må du kontrollere at du tilordner en lisens [til brukeren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Hvis brukeren har en lisens, bør du også kontrollere at de er tilordnet en [administratorrolle](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjonssentrene.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerprinsippnavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Pass unik ID). Når brukeren prøver å få tilgang til en områdesamling eller oneDrive, har brukeren feil PUID. En annen situasjon innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjonsadministrasjon og synkroniseres med SharePoint på nytt, kan de oppleve dette problemet.

Du kan løse dette problemet ved å gjenopprette det opprinnelige UPN-navnet ved hjelp av fremgangsmåten i artikkelen Gjenopprette en [bruker i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Obs! Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.  [Kontroller tilstandsinstrumentbordet](https://portal.office.com/adminportal/home#/servicehealth)for tjenesten.



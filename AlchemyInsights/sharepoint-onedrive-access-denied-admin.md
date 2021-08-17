---
title: Feilsøke meldinger som ikke får tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085237"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøke meldinger som ikke er tilgjengelig i Sharepoint/OneDrive-administrasjonssenteret

Hvis du mottar en melding om at du ikke får tilgang når du prøver å bla til et administrasjonssenter for Sharepoint/OneDrive, må du passe på at du tilordner en lisens [til brukeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Hvis brukeren har en lisens, bør du også kontrollere at de er tilordnet en [administratorrolle](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjonssentrene.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerprinsippnavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID). Når brukeren prøver å få tilgang til en nettstedssamling eller OneDrive, har brukeren feil PUID. Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjonsenheten og synkroniseres på nytt med SharePoint, kan de oppleve dette problemet.

Du kan løse dette problemet ved å gjenopprette det opprinnelige UPN-nummeret med fremgangsmåten i artikkelen Gjenopprette [en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Obs! Hvis et OneDrive eller SharePoint administrasjonssenter ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.  [Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).



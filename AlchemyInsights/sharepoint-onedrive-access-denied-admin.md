---
title: Feilsøke access avviste meldinger
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505388"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøke access avviste meldinger i administrasjonssenteret for Sharepoint/OneDrive

Hvis du mottar en melding om tilgang når du prøver å gå til et administrasjonssenter for Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjonssentrene.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID). Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID. Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjon og synkroniseres på nytt med SharePoint, kan det oppstå dette problemet.

Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i [artikkelen, Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Merk: Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.  [Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).



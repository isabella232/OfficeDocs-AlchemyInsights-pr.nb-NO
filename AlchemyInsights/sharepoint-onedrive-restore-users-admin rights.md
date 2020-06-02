---
title: Feilsøke access-avslåtte meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511193"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Feilsøke access-avslåtte meldinger til OneDrive for Business-områder

Dette problemet oppstår oftest når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID). Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID. Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjon og synkroniseres på nytt med SharePoint, kan det oppstå dette problemet.

1. Hvis du vil løse dette problemet, bør du gjenopprette det opprinnelige UPN med trinnene i artikkelen, [Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Hvis du ikke kan gjenopprette den opprinnelige brukeren, bør du fjerne den gamle brukeren fra OneDrive-området ved hjelp av disse trinnene, [fjerne en bruker fra brukerinformasjonslisten](). 
3. Når dette er gjort, kan du kontrollere at brukeren har administratorrettigheter til OneDrive-området ved å følge trinnene [for å legge til administratorer for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Hvis du vil ha mer informasjon om tillatelsesnivåer, kan du se artikkelen [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

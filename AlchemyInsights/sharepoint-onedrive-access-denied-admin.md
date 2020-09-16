---
title: Feilsøke meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767671"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Feilsøke tilgang til meldinger som nektes i administrasjons senteret for SharePoint/OneDrive

Hvis du mottar en melding om at du ikke får tilgang når du prøver å bla til et administrasjons senter for SharePoint/OneDrive, må du sørge for at du [tilordner en lisens til brukeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Hvis brukeren har en lisens, bør du også sørge for at de er [tilordnet en administrator rolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjons sentrene.

Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN). Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (konto – unik ID). Når brukeren prøver å få tilgang til en område samling eller deres OneDrive, har brukeren feil PUID. Et annet scenario omfatter katalog synkronisering med en Active Directory-organisasjonsenhet (OU). Hvis brukerne allerede har logget seg på SharePoint, og deretter flyttes til en annen OU og synkroniseres med SharePoint, kan de oppleve dette problemet.

Du kan løse dette problemet ved å gjenopprette den opprinnelige UPN-en med trinnene i artikkelen, [gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Obs! hvis et administrasjons senter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjeneste problem.  [Kontroller instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).



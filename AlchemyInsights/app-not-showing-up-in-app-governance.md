---
title: Appen min vises ikke i Appstyring
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454996"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Appen min vises ikke i Appstyring

Hvis programmet ikke vises i App governance, kontrollerer du følgende:

1. Gå til [Azure AD,](https://aad.portal.azure.com/) og finn app-ID-en for programmet ved å søke etter appnavnet i den øverste linjen på Oversikt-siden.

1. Access Graph Explorer, og søk etter app-ID-en i tjenesteprinsippet ved å bruke denne spørringen og erstatte med den relevante <appId> app-ID-en: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Hvis ingen resultater returneres, kan du søke etter app-ID-en i programmet ved hjelp av denne spørringen og erstatte med den relevante <appId> app-ID-en: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Hvis du opplever problemer med spørringen, kan du [se Få kundestøtte](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Hvis du vil ha mer informasjon eller innsikt i appene dine i Appstyring, kan du se Lær [om synlighet og innsikt.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Hvis du vil ha mer informasjon om hvordan du viser appene dine, kan [du se Vise appene dine](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).

---
title: Løse tilkoblingspolicy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888415"
---
# <a name="fix-connection-policy"></a>Løse tilkoblingspolicy

E-postmeldingen ble merket som sikker og levert til brukerens innboks fordi kilde-IP-adressen ble merket som sikker i standard policy for tilkoblingsfilter. Gjør følgende for å se gjennom policyen:

1. I Microsoft 365 Defender-portalen på går du til Policyer for e-& for samarbeid & policyer for trusler mot søppelpost i <https://security.microsoft.com/>  \>  \>  \>  **Policyer-delen.**

   Hvis du vil gå direkte til **siden for søppelpostpolicyer,** bruker du <https://security.microsoft.com/antispam> .

2. Velg **policyen** tilkoblingsfilterpolicy **(standard)** på siden Søppelpostpolicyer ved å klikke på navnet på policyen.

3. Klikk Rediger policy for tilkoblingsfilter i delen Tilkoblingsfiltrering på detaljer-undermenyen som vises.  

4. Se gjennom oppføringene i delen Tillat alltid meldinger fra følgende **IP-adresser** eller adresseområde, og se om **Aktiver sikker-listen** er valgt.

   > [!NOTE]
   > Microsoft abonnerer på tredjepartskilder for klarerte avsendere. Hvis listen over klarerte avsendere er aktivert, merkes ikke disse klarerte avsenderne feilaktig som søppelpost. Vi anbefaler at du velger dette alternativet, fordi det vil redusere antall falske positiver (god e-post som er klassifisert som søppelpost) som du mottar.

Hvis du vil ha mer informasjon, kan [du se Konfigurere tilkoblingsfiltrering](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).

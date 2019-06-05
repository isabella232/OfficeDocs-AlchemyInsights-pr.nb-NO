---
title: Opprette og bruke en delt postboks
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717355"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøke problemet - brukeren ble ikke funnet i katalogen

<p>Hvis brukere får feilmeldingen <strong> &ldquo; &hellip;kan brukeren&rsquo;t finnes i katalogen. Prøv&hellip; </strong> der problemet er <strong> &ldquo;bruker ikke i katalogen.&rdquo;</strong>, kan fullføre trinnene nedenfor for å feilsøke problemet.</p> <ol> <li>Sikre at kontoen som godkjent e-postinvitasjonen er den samme kontoen som brukes til å logge på igjen senere. Kontroller at du bruker samme konto til å godta invitasjonen og logge inn på området. <br /><br />For mer informasjon, se <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">Administrere aliaser for Microsoft-konto</a> til å administrere Office 365-pålogging. <br /><br /></li> <li>Bla til hver område(r) der brukeren mottar feilen. <br /><br />en. Legge til <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (i de doble anførselstegnene) på slutten av URL-adressen for området. <br /><br />Eksempel: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Velg brukeren fra listen. <br /><br />c. Klikk <strong>Fjern brukertillatelser fra båndet</strong>. <br /><br />d. Legge tilbake til brukeren, og Send invitasjonen på nytt til brukeren.</li> </ol>


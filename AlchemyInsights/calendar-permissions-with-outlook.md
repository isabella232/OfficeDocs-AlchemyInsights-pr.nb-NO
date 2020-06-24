---
title: Kalendertillatelser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862173"
---
# <a name="calendar-permissions"></a><span data-ttu-id="80900-102">Kalendertillatelser</span><span class="sxs-lookup"><span data-stu-id="80900-102">Calendar Permissions</span></span>

<span data-ttu-id="80900-103">Brukere kan endre sine egne kalendertillatelser med Outlook på nettet eller andre klienter, men som administrator må du kanskje undersøke også.</span><span class="sxs-lookup"><span data-stu-id="80900-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="80900-104">Med Exchange PowerShell-cmdleten vil vise deg tillatelsen på en brukers kalender:</span><span class="sxs-lookup"><span data-stu-id="80900-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="80900-105">Hvis du vil ha mer informasjon, kan du se følgende:</span><span class="sxs-lookup"><span data-stu-id="80900-105">To see more information see the following:</span></span>

- [<span data-ttu-id="80900-106">Få mailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="80900-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="80900-107">Sett mailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="80900-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="80900-108">Legg til MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="80900-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="80900-109">Kalendertillatelser brukes i deling av kalendere for å se mer informasjon om deling av en Outlook-kalender, se disse artiklene:</span><span class="sxs-lookup"><span data-stu-id="80900-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="80900-110">Dele en Outlook-kalender med andre</span><span class="sxs-lookup"><span data-stu-id="80900-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="80900-111">Dele kalenderen i Outlook på nettet for bedrifter</span><span class="sxs-lookup"><span data-stu-id="80900-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="80900-112">Hvis du vil feilsøke kalendertillatelse, kan du bruke verktøyet [Støtte- og gjenopprettingsassistent.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="80900-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>
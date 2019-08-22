---
title: Feilsøke problemer med «Åpne med Utforsker» i SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 52429314d1529d0d2df7886feaebbcfd27666a06
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559706"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="bb093-102">Feilsøke problemer med «Åpne med Utforsker» i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bb093-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="bb093-103">Kommandoen Åpne med Utforsker åpner en lokal forekomst av Windows Utforsker som viser mappestrukturen på serveren som er vert for SharePoint-området.</span><span class="sxs-lookup"><span data-stu-id="bb093-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="bb093-104">Vi anbefaler imidlertid at du [synkroniserer SharePoint-filer med den nye synkroniseringsklienten for OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> som gir tilgang til [filer ved behov](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), fordi den gir lokal tilgang til filene og tilbyr den beste ytelsen.</span><span class="sxs-lookup"><span data-stu-id="bb093-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="bb093-105">Hvis du valgte å bruke Utforsker-visning i stedet for å bruke den nye synkroniseringsklienten for OneDrive, må du passe på at du følger trinnene og de anbefalte fremgangsmåtene i artiklene nedenfor:</span><span class="sxs-lookup"><span data-stu-id="bb093-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="bb093-106">Slik bruker du kommandoen Åpne med Utforsker til å feilsøke problemer i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bb093-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="bb093-107">Kopiere eller flytte bibliotekfiler ved å bruke Åpne med Utforsker</span><span class="sxs-lookup"><span data-stu-id="bb093-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="bb093-108">**Åpne med Utforsker**-knappen vises ikke i den nye bibliotekopplevelsen</span><span class="sxs-lookup"><span data-stu-id="bb093-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="bb093-109">Velg **Vis** rullegardinmenyen oppe til høyre (navnet på rullegardinmenyen endres basert på gjeldende visning), og velg deretter **Vis i Filutforsker**.</span><span class="sxs-lookup"><span data-stu-id="bb093-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="bb093-110">SharePoint Åpne med Utforsker bruker ActiveX-kontroller, så det støttes bare i Internet Explorer 10 eller 11.</span><span class="sxs-lookup"><span data-stu-id="bb093-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="bb093-111">Åpne med Utforsker virker ikke i Windows med Microsoft Edge, Google Chrome, Mozilla Firefox eller på Mac-plattformen.</span><span class="sxs-lookup"><span data-stu-id="bb093-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="bb093-112">På grunn av dette kan det hende at alternativet Utforsker-visning er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="bb093-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="bb093-113">[Hvorfor er SharePoint-båndknapper utilgjengelige eller nedtonet](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="bb093-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  


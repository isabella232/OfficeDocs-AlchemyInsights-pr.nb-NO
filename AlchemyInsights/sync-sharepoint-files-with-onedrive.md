---
title: Feilsøke problemer med «Åpne med Explorer» i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: fcaca189741bd68878b1dcfab879e6e0f64e6794
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223649"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="80325-102">Feilsøke problemer med «Åpne med Explorer» i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="80325-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="80325-103">Kommandoen Åpne med Explorer åpner en lokal forekomst av Windows Utforsker som viser mappestrukturen på serveren som er vert for SharePoint-området.</span><span class="sxs-lookup"><span data-stu-id="80325-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="80325-104">Vi anbefaler imidlertid at du [synkroniserer SharePoint-filer med den nye synkroniseringsklienten for OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> som gir tilgang til [filer ved behov](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), fordi den gir lokal tilgang til filene og tilbyr den beste ytelsen.</span><span class="sxs-lookup"><span data-stu-id="80325-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="80325-105">Hvis du valgte å bruke utforskervisningen i stedet for å bruke den nye synkroniseringsklienten, må du passe på at du følger trinnene og gode fremgangsmåter i artiklene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="80325-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="80325-106">Slik bruker du kommandoen Åpne med Utforsker til å feilsøke problemer i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="80325-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="80325-107">Kopiere eller flytte bibliotekfiler ved å bruke Åpne med Explorer</span><span class="sxs-lookup"><span data-stu-id="80325-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="80325-108">Obs! Åpne med Utforsker-knappen vises ikke i den nye bibliotekopplevelsen</span><span class="sxs-lookup"><span data-stu-id="80325-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="80325-109">Klikk på Vis-rullegardinmenyen oppe til høyre (navnet på rullegardinmenyen endres basert på gjeldende visning), og klikk på Vis i Filutforsker.</span><span class="sxs-lookup"><span data-stu-id="80325-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="80325-110">SharePoint Åpne med Explorer bruker ActiveX-kontroller, så det støttes bare i Internet Explorer 10 eller 11.</span><span class="sxs-lookup"><span data-stu-id="80325-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="80325-111">Åpne med Explorer virker ikke i Windows med Microsoft Edge, Google Chrome, Mozilla Firefox eller på Mac-plattformen.</span><span class="sxs-lookup"><span data-stu-id="80325-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="80325-112">På grunn av dette kan det hende at alternativet Explorer-visning er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="80325-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="80325-113">[Hvorfor er SharePoint-båndknapper utilgjengelige eller nedtonet](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="80325-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  


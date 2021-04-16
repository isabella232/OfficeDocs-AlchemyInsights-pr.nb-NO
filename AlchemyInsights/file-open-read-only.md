---
title: Åpne fil skrivebeskyttet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813193"
---
# <a name="file-open-read-only"></a><span data-ttu-id="63916-102">Åpne fil skrivebeskyttet</span><span class="sxs-lookup"><span data-stu-id="63916-102">File open read-only</span></span>

<span data-ttu-id="63916-103">Det kan hende at når du åpner filer, åpnes de som skrivebeskyttet.</span><span class="sxs-lookup"><span data-stu-id="63916-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="63916-104">I noen tilfeller er dette for ekstra sikkerhet, for eksempel når du åpner filer fra Internett og andre ganger, kan det være på grunn av en innstilling som kan endres.</span><span class="sxs-lookup"><span data-stu-id="63916-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="63916-105">Her er noen scenarioer der en fil åpnes skrivebeskyttet, og noen trinn du kan gjøre for å endre dette.</span><span class="sxs-lookup"><span data-stu-id="63916-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="63916-106">**Antivirusprogrammet mitt gjør at de åpner skrivebeskyttet**</span><span class="sxs-lookup"><span data-stu-id="63916-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="63916-107">Noen antivirusprogrammer kan beskytte deg mot potensielt usikre filer ved å åpne dem skrivebeskyttet.</span><span class="sxs-lookup"><span data-stu-id="63916-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="63916-108">Du må kanskje ta kontakt med antivirusleverandøren for å finne ut hvordan du justerer disse innstillingene.</span><span class="sxs-lookup"><span data-stu-id="63916-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="63916-109">BitDefender har for eksempel innhold om å legge til programekskluderinger her: Slik legger du til program- eller [prosessekskluderinger i Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="63916-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="63916-110">**Er filegenskapene satt til skrivebeskyttet?**</span><span class="sxs-lookup"><span data-stu-id="63916-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="63916-111">Du kan kontrollere filegenskapene ved å høyreklikke på filen og velge Egenskaper.</span><span class="sxs-lookup"><span data-stu-id="63916-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="63916-112">Hvis skrivebeskyttet-attributtet er avmerket, kan du fjerne merket for det og klikke OK.</span><span class="sxs-lookup"><span data-stu-id="63916-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="63916-113">**Innholdet er i beskyttet visning**</span><span class="sxs-lookup"><span data-stu-id="63916-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="63916-114">Filer fra Internett og andre potensielt usikre plasseringer kan inneholde virus, ormer eller andre typer skadelig programvare som kan skade datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="63916-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="63916-115">Dette er også vanlig med e-postvedlegg eller filer du har lastet ned.</span><span class="sxs-lookup"><span data-stu-id="63916-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="63916-116">Filer fra disse potensielt usikre plasseringene åpnes i beskyttet visning for å beskytte datamaskinen.</span><span class="sxs-lookup"><span data-stu-id="63916-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="63916-117">Ved hjelp av beskyttet visning kan du lese en fil og se innholdet samtidig som du reduserer risikoene.</span><span class="sxs-lookup"><span data-stu-id="63916-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="63916-118">Hvis du vil ha mer informasjon om beskyttet visning og hvordan du endrer innstillinger, kan du se denne artikkelen: [Hva er beskyttet visning?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="63916-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="63916-119">**Er OneDrive full?**</span><span class="sxs-lookup"><span data-stu-id="63916-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="63916-120">Hvis filen er lagret på OneDrive og OneDrive-lagringsplassen er full, kan du ikke lagre dokumentet før du er under den tildelte plassen.</span><span class="sxs-lookup"><span data-stu-id="63916-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="63916-121">Du kan kontrollere ledig plass på OneDrive ved å klikke OneDrive-ikonet i varslingssenteret og velge Administrer lagringsplass, eller du kan gå til , logge på og notere hvor mye brukt plass som er nede til venstre på [https://onedrive.live.com](https://onedrive.live.com) skjermen.</span><span class="sxs-lookup"><span data-stu-id="63916-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="63916-122">**Er Office aktivert?**</span><span class="sxs-lookup"><span data-stu-id="63916-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="63916-123">Hvis Office ikke er aktivert, eller hvis abonnementet er utløpt, kan du være i skrivebeskyttet modus for redusert funksjonalitet.</span><span class="sxs-lookup"><span data-stu-id="63916-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="63916-124">Hvis du vil ha informasjon om hvordan du aktiverer Office, kan du se: Feil med ulisensiert [produkt og aktivering i Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="63916-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="63916-125">**Hvis alt annet mislykkes ...**</span><span class="sxs-lookup"><span data-stu-id="63916-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="63916-126">Prøv å starte datamaskinen på nytt</span><span class="sxs-lookup"><span data-stu-id="63916-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="63916-127">Installere Office-oppdateringer</span><span class="sxs-lookup"><span data-stu-id="63916-127">Install Office updates</span></span>
    
- <span data-ttu-id="63916-128">Utføre en tilkoblet reparasjon av Office</span><span class="sxs-lookup"><span data-stu-id="63916-128">Perform an Online repair of Office</span></span>
    


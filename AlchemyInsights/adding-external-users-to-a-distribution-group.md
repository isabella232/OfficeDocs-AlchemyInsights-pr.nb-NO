---
title: Legge til eksterne brukere i en distribusjonsgruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910941"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="7714e-102">Legge til eksterne brukere i en distribusjonsgruppe</span><span class="sxs-lookup"><span data-stu-id="7714e-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="7714e-103">Legge til en ekstern kontakt i en distribusjonsgruppe (DG) er en to-trinns prosess:</span><span class="sxs-lookup"><span data-stu-id="7714e-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="7714e-104">Opprett en e-postkontakt for den eksterne brukeren:</span><span class="sxs-lookup"><span data-stu-id="7714e-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="7714e-105">Gå til **Brukere** > [kontakter-siden](https://admin.microsoft.com/adminportal/home#/Contact) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="7714e-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="7714e-106">Velg **Legg til en kontakt**.</span><span class="sxs-lookup"><span data-stu-id="7714e-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="7714e-107">Skriv inn informasjonen for kontakten, og velg **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="7714e-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="7714e-108">Legg til e-postkontakten i DG:</span><span class="sxs-lookup"><span data-stu-id="7714e-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="7714e-109">Gå til > [Gruppergrupper-siden](https://admin.microsoft.com/adminportal/home#/groups) i administrasjonssenteret. **Groups**</span><span class="sxs-lookup"><span data-stu-id="7714e-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="7714e-110">Finn DG du vil legge til den eksterne brukeren i, og velg den for å åpne redigeringsdialogboksen.</span><span class="sxs-lookup"><span data-stu-id="7714e-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="7714e-111">Velg Vis alle på **Medlemmer-fanen,** **og administrer medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="7714e-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="7714e-112">Velg **Legg til medlemmer**.</span><span class="sxs-lookup"><span data-stu-id="7714e-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="7714e-113">Velg e-postkontakten du opprettet i forrige trinn, og velg deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="7714e-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="7714e-114">Hvis de eksterne brukerne ikke kan sende e-post til DG eller ikke motta e-post fra den etter å ha fulgt disse trinnene, kan ikke sende e-post til DG eller ikke motta e-post fra den, men det kan være at DG er merket for å bare tillate e-post fra interne brukere.</span><span class="sxs-lookup"><span data-stu-id="7714e-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="7714e-115">Du kan sjekke denne konfigurasjonen og fikse den ved å følge instruksjonene [her](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="7714e-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="7714e-116">**Merk:** Disse instruksjonene gjelder ikke hvis gruppens type er "Microsoft 365-gruppe" i stedet for "Distribusjonsgruppe".</span><span class="sxs-lookup"><span data-stu-id="7714e-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="7714e-117">Hvis det er tilfelle, kan du legge til den eksterne brukeren direkte i gruppen fra Outlook.</span><span class="sxs-lookup"><span data-stu-id="7714e-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="7714e-118">Detaljert informasjon om Microsoft 365 Grupper gjester samt instruksjoner for å legge til eksterne gjester kan bli funnet i [denne artikkelen](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="7714e-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  
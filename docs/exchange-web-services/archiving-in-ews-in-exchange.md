---
title: Exchange での EWS のアーカイブ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Exchange での EWS のアーカイブについて説明します。
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758871"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="ac6b8-103">Exchange での EWS のアーカイブ</span><span class="sxs-lookup"><span data-stu-id="ac6b8-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="ac6b8-104">Exchange での EWS のアーカイブについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="ac6b8-p101">アーカイブ メールボックスは、ユーザーに関連付けられている 2 番目のメールボックスです。通常、アーカイブ メールボックスはメールの格納域の制限に対処するために使用されます。たとえば、古いメール アイテムは、定期的に受信トレイからアーカイブ メールボックスに移動されます。 </span><span class="sxs-lookup"><span data-stu-id="ac6b8-p101">Archive mailboxes are secondary mailboxes that are associated with a user. Archive mailboxes are typically used to manage email storage limits. For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="ac6b8-108">Exchange のオンライン、Office 365、および Exchange Server 2013 の一部として Exchange Online は、一連のプライマリ メールボックスからメール アイテムをアーカイブするために使用できる 2 つの新しい Exchange Web サービス (EWS) 操作を紹介します。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="ac6b8-109">この方法で受信トレイのアイテムをアーカイブには、アイテムのフォルダー階層が保持されます。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="ac6b8-110">さらに、アーカイブ メールボックス格納できるよう、クライアントにローカルでまたはリモートでは、アーカイブのコンテンツをポイントするフォルダーのパスを使用してユーザーに不透明なほとんどの方法で。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="ac6b8-111">EWS でのアーカイブ操作</span><span class="sxs-lookup"><span data-stu-id="ac6b8-111">Archiving operations in EWS</span></span>

<span data-ttu-id="ac6b8-112">次の表に、Exchange 2013 で導入されたアーカイブ ・ オペレーションを示します。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="ac6b8-113">**操作名**</span><span class="sxs-lookup"><span data-stu-id="ac6b8-113">**Operation name**</span></span>|<span data-ttu-id="ac6b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ac6b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac6b8-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ac6b8-115">ArchiveItem</span></span>](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="ac6b8-116">アイテムをプライマリ メールボックスからアーカイブ メールボックスに移動します。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ac6b8-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="ac6b8-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="ac6b8-118">アーカイブ メールボックスの格納場所をポイントする URI を作成します。</span><span class="sxs-lookup"><span data-stu-id="ac6b8-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac6b8-119">関連項目</span><span class="sxs-lookup"><span data-stu-id="ac6b8-119">See also</span></span>

- [<span data-ttu-id="ac6b8-120">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="ac6b8-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="ac6b8-121">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="ac6b8-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="ac6b8-122">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="ac6b8-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    


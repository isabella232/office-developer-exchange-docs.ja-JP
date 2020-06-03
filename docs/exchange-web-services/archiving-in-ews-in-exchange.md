---
title: Exchange での EWS のアーカイブ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Exchange での EWS のアーカイブについて説明します。
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456214"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="df443-103">Exchange での EWS のアーカイブ</span><span class="sxs-lookup"><span data-stu-id="df443-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="df443-104">Exchange での EWS のアーカイブについて説明します。</span><span class="sxs-lookup"><span data-stu-id="df443-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="df443-p101">アーカイブ メールボックスは、ユーザーに関連付けられている 2 番目のメールボックスです。通常、アーカイブ メールボックスはメールの格納域の制限に対処するために使用されます。たとえば、古いメール アイテムは、定期的に受信トレイからアーカイブ メールボックスに移動されます。 </span><span class="sxs-lookup"><span data-stu-id="df443-p101">Archive mailboxes are secondary mailboxes that are associated with a user. Archive mailboxes are typically used to manage email storage limits. For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="df443-108">Exchange Online、Office 365 の一部としての Exchange Online、および Exchange Server 2013 は、2 つの新しい Exchange Web サービス (EWS) 操作を導入し、これらを使用してプライマリ メールボックスからメール アイテムのセットをアーカイブできます。</span><span class="sxs-lookup"><span data-stu-id="df443-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="df443-109">この方法で受信トレイのアイテムをアーカイブすると、アイテムのフォルダー階層が保持されます。</span><span class="sxs-lookup"><span data-stu-id="df443-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="df443-110">さらに、アーカイブ メールボックスを、クライアント上にローカルに格納することもリモートで格納することもできるようなりました。その際、アーカイブのコンテンツを指すフォルダー パスを使用し、ユーザーにはほとんど見えない方法で行うことができます。</span><span class="sxs-lookup"><span data-stu-id="df443-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="df443-111">EWS でのアーカイブ操作</span><span class="sxs-lookup"><span data-stu-id="df443-111">Archiving operations in EWS</span></span>

<span data-ttu-id="df443-112">次の表に、Exchange 2013 で導入されたアーカイブ操作を記載します。</span><span class="sxs-lookup"><span data-stu-id="df443-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="df443-113">**操作名**</span><span class="sxs-lookup"><span data-stu-id="df443-113">**Operation name**</span></span>|<span data-ttu-id="df443-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="df443-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df443-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="df443-115">ArchiveItem</span></span>](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="df443-116">アイテムをプライマリ メールボックスからアーカイブ メールボックスに移動します。</span><span class="sxs-lookup"><span data-stu-id="df443-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="df443-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="df443-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="df443-118">アーカイブ メールボックスの格納場所をポイントする URI を作成します。</span><span class="sxs-lookup"><span data-stu-id="df443-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df443-119">関連項目</span><span class="sxs-lookup"><span data-stu-id="df443-119">See also</span></span>

- [<span data-ttu-id="df443-120">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="df443-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="df443-121">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="df443-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="df443-122">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="df443-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    


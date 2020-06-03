---
title: UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: c6ae99c4-18b0-4136-90ab-12cf15e15f91
description: UpdateDelegate 要素は、メールボックス内の代理人を更新する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 17d69eb8c539217d39e1dd0c2616261d02ad304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468874"
---
# <a name="updatedelegate"></a><span data-ttu-id="db5d1-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="db5d1-104">UpdateDelegate</span></span>

<span data-ttu-id="db5d1-105">**Updatedelegate**要素は、メールボックス内の代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="db5d1-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="db5d1-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db5d1-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="db5d1-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="db5d1-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db5d1-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="db5d1-108">Attributes and elements</span></span>

<span data-ttu-id="db5d1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db5d1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db5d1-110">属性</span><span class="sxs-lookup"><span data-stu-id="db5d1-110">Attributes</span></span>

<span data-ttu-id="db5d1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="db5d1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db5d1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="db5d1-112">Child elements</span></span>

|<span data-ttu-id="db5d1-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="db5d1-113">**Element**</span></span>|<span data-ttu-id="db5d1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="db5d1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db5d1-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="db5d1-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="db5d1-116">代理人と代理人に適用する更新プログラムを識別する[DelegateUser](delegateuser.md)要素の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="db5d1-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="db5d1-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db5d1-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="db5d1-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="db5d1-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="db5d1-119">代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="db5d1-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="db5d1-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db5d1-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="db5d1-121">メールボックス</span><span class="sxs-lookup"><span data-stu-id="db5d1-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="db5d1-122">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="db5d1-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db5d1-123">親要素</span><span class="sxs-lookup"><span data-stu-id="db5d1-123">Parent elements</span></span>

<span data-ttu-id="db5d1-124">なし。</span><span class="sxs-lookup"><span data-stu-id="db5d1-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db5d1-125">注釈</span><span class="sxs-lookup"><span data-stu-id="db5d1-125">Remarks</span></span>

<span data-ttu-id="db5d1-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="db5d1-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db5d1-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="db5d1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db5d1-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="db5d1-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db5d1-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db5d1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="db5d1-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="db5d1-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="db5d1-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db5d1-131">Validation File</span></span>  <br/> |<span data-ttu-id="db5d1-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="db5d1-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db5d1-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db5d1-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="db5d1-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="db5d1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db5d1-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="db5d1-135">See also</span></span>



[<span data-ttu-id="db5d1-136">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="db5d1-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="db5d1-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="db5d1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: UpdateDelegate 要素は、メールボックスの代理人を更新する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 32322e48acfa5f1058786162565a185a3e565d6e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839830"
---
# <a name="updatedelegate"></a><span data-ttu-id="b9a3e-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b9a3e-104">UpdateDelegate</span></span>

<span data-ttu-id="b9a3e-105">**UpdateDelegate**要素は、メールボックスの代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="b9a3e-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="b9a3e-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="b9a3e-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9a3e-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b9a3e-108">Attributes and elements</span></span>

<span data-ttu-id="b9a3e-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9a3e-110">属性</span><span class="sxs-lookup"><span data-stu-id="b9a3e-110">Attributes</span></span>

<span data-ttu-id="b9a3e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9a3e-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b9a3e-112">Child elements</span></span>

|<span data-ttu-id="b9a3e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9a3e-113">**Element**</span></span>|<span data-ttu-id="b9a3e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9a3e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a3e-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="b9a3e-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="b9a3e-116">代理人および代理人に適用する更新プログラムを識別する[DelegateUser](delegateuser.md)の要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="b9a3e-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b9a3e-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="b9a3e-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="b9a3e-119">主体と代理人の間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="b9a3e-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b9a3e-121">メールボックス</span><span class="sxs-lookup"><span data-stu-id="b9a3e-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b9a3e-122">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9a3e-123">親要素</span><span class="sxs-lookup"><span data-stu-id="b9a3e-123">Parent elements</span></span>

<span data-ttu-id="b9a3e-124">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9a3e-125">備考</span><span class="sxs-lookup"><span data-stu-id="b9a3e-125">Remarks</span></span>

<span data-ttu-id="b9a3e-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b9a3e-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9a3e-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="b9a3e-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9a3e-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="b9a3e-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9a3e-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9a3e-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b9a3e-130">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9a3e-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9a3e-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9a3e-131">Validation File</span></span>  <br/> |<span data-ttu-id="b9a3e-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9a3e-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9a3e-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b9a3e-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9a3e-134">False</span><span class="sxs-lookup"><span data-stu-id="b9a3e-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9a3e-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9a3e-135">See also</span></span>



[<span data-ttu-id="b9a3e-136">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="b9a3e-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="b9a3e-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b9a3e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: AddDelegate 要素は、メールボックスに代理人を追加する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: a08b83ad6e114c194073716c82228ea20ae1d3b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466501"
---
# <a name="adddelegate"></a><span data-ttu-id="3dcde-104">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="3dcde-104">AddDelegate</span></span>

<span data-ttu-id="3dcde-105">**Adddelegate**要素は、メールボックスに代理人を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3dcde-105">The **AddDelegate** element defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="3dcde-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3dcde-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 <span data-ttu-id="3dcde-107">**AddDelegateType**</span><span class="sxs-lookup"><span data-stu-id="3dcde-107">**AddDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dcde-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3dcde-108">Attributes and elements</span></span>

<span data-ttu-id="3dcde-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3dcde-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dcde-110">属性</span><span class="sxs-lookup"><span data-stu-id="3dcde-110">Attributes</span></span>

<span data-ttu-id="3dcde-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3dcde-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dcde-112">子要素</span><span class="sxs-lookup"><span data-stu-id="3dcde-112">Child elements</span></span>

|<span data-ttu-id="3dcde-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="3dcde-113">**Element**</span></span>|<span data-ttu-id="3dcde-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3dcde-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dcde-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="3dcde-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="3dcde-116">メールボックスに追加または更新する代理人の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3dcde-116">Contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="3dcde-117">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3dcde-117">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="3dcde-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="3dcde-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="3dcde-119">代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="3dcde-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="3dcde-120">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3dcde-120">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="3dcde-121">メールボックス</span><span class="sxs-lookup"><span data-stu-id="3dcde-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3dcde-122">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="3dcde-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3dcde-123">親要素</span><span class="sxs-lookup"><span data-stu-id="3dcde-123">Parent elements</span></span>

<span data-ttu-id="3dcde-124">なし。</span><span class="sxs-lookup"><span data-stu-id="3dcde-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3dcde-125">注釈</span><span class="sxs-lookup"><span data-stu-id="3dcde-125">Remarks</span></span>

<span data-ttu-id="3dcde-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="3dcde-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3dcde-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3dcde-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dcde-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dcde-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3dcde-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3dcde-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3dcde-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3dcde-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3dcde-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3dcde-131">Validation File</span></span>  <br/> |<span data-ttu-id="3dcde-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3dcde-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dcde-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3dcde-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dcde-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="3dcde-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dcde-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="3dcde-135">See also</span></span>

- [<span data-ttu-id="3dcde-136">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3dcde-136">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="3dcde-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3dcde-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3dcde-138">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="3dcde-138">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


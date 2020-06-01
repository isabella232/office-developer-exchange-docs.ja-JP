---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: ReceiveCopiesOfMeetingMessages 要素は、代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: af6e220304f88c4db00ab675077dcd9bf581ea9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468265"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="8e019-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="8e019-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="8e019-105">**ReceiveCopiesOfMeetingMessages**要素は、代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8e019-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="8e019-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e019-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="8e019-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8e019-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e019-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e019-108">Attributes and elements</span></span>

<span data-ttu-id="8e019-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e019-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e019-110">属性</span><span class="sxs-lookup"><span data-stu-id="8e019-110">Attributes</span></span>

<span data-ttu-id="8e019-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8e019-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e019-112">子要素</span><span class="sxs-lookup"><span data-stu-id="8e019-112">Child elements</span></span>

<span data-ttu-id="8e019-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8e019-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e019-114">親要素</span><span class="sxs-lookup"><span data-stu-id="8e019-114">Parent elements</span></span>

|<span data-ttu-id="8e019-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e019-115">**Element**</span></span>|<span data-ttu-id="8e019-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e019-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e019-117">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="8e019-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="8e019-118">メールボックスに追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e019-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="8e019-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8e019-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e019-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e019-120">Text value</span></span>

<span data-ttu-id="8e019-121">テキスト値が**true の場合**は、代理人が会議メッセージのコピーを受信することを示します。</span><span class="sxs-lookup"><span data-stu-id="8e019-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="8e019-122">テキスト値が**false**の場合は、代理人が会議メッセージのコピーを受信しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8e019-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8e019-123">注釈</span><span class="sxs-lookup"><span data-stu-id="8e019-123">Remarks</span></span>

<span data-ttu-id="8e019-124">**ReceiveCopiesOfMeetingMessages**が**false**に設定されている場合でも、代理人はプリンシパルに代わってメッセージを送信できますが、会議関連のメッセージを受信することはありません。</span><span class="sxs-lookup"><span data-stu-id="8e019-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="8e019-125">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="8e019-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e019-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8e019-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e019-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e019-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e019-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8e019-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8e019-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8e019-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e019-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8e019-130">Validation File</span></span>  <br/> |<span data-ttu-id="8e019-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8e019-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e019-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8e019-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e019-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="8e019-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e019-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e019-134">See also</span></span>



[<span data-ttu-id="8e019-135">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="8e019-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="8e019-136">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="8e019-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="8e019-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e019-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8e019-138">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="8e019-138">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


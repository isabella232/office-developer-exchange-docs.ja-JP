---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: GetDelegate 要素は、メールボックスへの代理人に関する情報を取得する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: bd7fb55800b51eb2d69184bc4e04cdef3e6b9a89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461031"
---
# <a name="getdelegate"></a><span data-ttu-id="bd791-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="bd791-104">GetDelegate</span></span>

<span data-ttu-id="bd791-105">**Getdelegate**要素は、メールボックスへの代理人に関する情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="bd791-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="bd791-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bd791-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="bd791-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="bd791-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd791-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bd791-108">Attributes and elements</span></span>

<span data-ttu-id="bd791-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd791-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd791-110">属性</span><span class="sxs-lookup"><span data-stu-id="bd791-110">Attributes</span></span>

|<span data-ttu-id="bd791-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="bd791-111">**Attribute**</span></span>|<span data-ttu-id="bd791-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd791-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd791-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="bd791-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="bd791-114">応答に各代理ユーザーのアクセス許可の設定が含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bd791-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="bd791-115">IncludePermissions 属性の値</span><span class="sxs-lookup"><span data-stu-id="bd791-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="bd791-116">**値**</span><span class="sxs-lookup"><span data-stu-id="bd791-116">**Value**</span></span>|<span data-ttu-id="bd791-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd791-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd791-118">**True**</span><span class="sxs-lookup"><span data-stu-id="bd791-118">**True**</span></span> <br/> |<span data-ttu-id="bd791-119">[UserId](userid.md)要素で返される代理人のユーザー情報に加えて、代理人のユーザー権限も返されます。</span><span class="sxs-lookup"><span data-stu-id="bd791-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="bd791-120">**False**</span><span class="sxs-lookup"><span data-stu-id="bd791-120">**False**</span></span> <br/> |<span data-ttu-id="bd791-121">[UserId](userid.md)情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="bd791-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bd791-122">子要素</span><span class="sxs-lookup"><span data-stu-id="bd791-122">Child elements</span></span>

|<span data-ttu-id="bd791-123">**Element**</span><span class="sxs-lookup"><span data-stu-id="bd791-123">**Element**</span></span>|<span data-ttu-id="bd791-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd791-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd791-125">メールボックス</span><span class="sxs-lookup"><span data-stu-id="bd791-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="bd791-126">プリンシパルのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="bd791-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bd791-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="bd791-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="bd791-128">プリンシパルのメールボックスから取得するデリゲートユーザーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="bd791-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="bd791-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bd791-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd791-130">親要素</span><span class="sxs-lookup"><span data-stu-id="bd791-130">Parent elements</span></span>

<span data-ttu-id="bd791-131">なし。</span><span class="sxs-lookup"><span data-stu-id="bd791-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd791-132">注釈</span><span class="sxs-lookup"><span data-stu-id="bd791-132">Remarks</span></span>

<span data-ttu-id="bd791-133">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="bd791-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd791-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bd791-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd791-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd791-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd791-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd791-136">Schema Name</span></span>  <br/> |<span data-ttu-id="bd791-137">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bd791-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd791-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd791-138">Validation File</span></span>  <br/> |<span data-ttu-id="bd791-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bd791-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd791-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd791-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd791-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="bd791-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd791-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd791-142">See also</span></span>



[<span data-ttu-id="bd791-143">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="bd791-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="bd791-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bd791-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


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
description: GetDelegate 要素は、メールボックスへの代理人についての情報を取得する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760687"
---
# <a name="getdelegate"></a><span data-ttu-id="3d7b2-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="3d7b2-104">GetDelegate</span></span>

<span data-ttu-id="3d7b2-105">**GetDelegate**要素は、メールボックスへの代理人についての情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="3d7b2-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="3d7b2-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d7b2-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3d7b2-108">Attributes and elements</span></span>

<span data-ttu-id="3d7b2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d7b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="3d7b2-110">Attributes</span></span>

|<span data-ttu-id="3d7b2-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-111">**Attribute**</span></span>|<span data-ttu-id="3d7b2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d7b2-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="3d7b2-114">代理人のユーザーごとにアクセス許可の設定が応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="3d7b2-115">IncludePermissions 属性の値</span><span class="sxs-lookup"><span data-stu-id="3d7b2-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="3d7b2-116">**値**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-116">**Value**</span></span>|<span data-ttu-id="3d7b2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d7b2-118">**True**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-118">**True**</span></span> <br/> |<span data-ttu-id="3d7b2-119">[ユーザー Id](userid.md)要素に返されるデリゲートのユーザー情報の他のアクセス許可が返されるユーザーに委任できます。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="3d7b2-120">**False**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-120">**False**</span></span> <br/> |<span data-ttu-id="3d7b2-121">[ユーザー Id](userid.md)情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3d7b2-122">子要素</span><span class="sxs-lookup"><span data-stu-id="3d7b2-122">Child elements</span></span>

|<span data-ttu-id="3d7b2-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-123">**Element**</span></span>|<span data-ttu-id="3d7b2-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d7b2-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d7b2-125">メールボックス</span><span class="sxs-lookup"><span data-stu-id="3d7b2-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3d7b2-126">主体のメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3d7b2-127">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="3d7b2-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="3d7b2-128">代理人のユーザー主体のメールボックスから取得する配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="3d7b2-129">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d7b2-130">親要素</span><span class="sxs-lookup"><span data-stu-id="3d7b2-130">Parent elements</span></span>

<span data-ttu-id="3d7b2-131">なし。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3d7b2-132">備考</span><span class="sxs-lookup"><span data-stu-id="3d7b2-132">Remarks</span></span>

<span data-ttu-id="3d7b2-133">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3d7b2-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d7b2-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="3d7b2-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d7b2-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="3d7b2-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3d7b2-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3d7b2-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3d7b2-137">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3d7b2-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3d7b2-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3d7b2-138">Validation File</span></span>  <br/> |<span data-ttu-id="3d7b2-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3d7b2-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d7b2-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3d7b2-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d7b2-141">False</span><span class="sxs-lookup"><span data-stu-id="3d7b2-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d7b2-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="3d7b2-142">See also</span></span>



[<span data-ttu-id="3d7b2-143">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="3d7b2-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="3d7b2-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3d7b2-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


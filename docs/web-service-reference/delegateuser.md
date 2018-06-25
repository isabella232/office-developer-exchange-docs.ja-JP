---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: DelegateUser の要素が 1 つのデリゲートを追加するメールボックスの更新を識別または代理人の管理の応答で、デリゲートが返されます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759954"
---
# <a name="delegateuser"></a><span data-ttu-id="52faa-104">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="52faa-104">DelegateUser</span></span>

<span data-ttu-id="52faa-105">**DelegateUser**の要素が 1 つのデリゲートを追加するメールボックスの更新を識別または代理人の管理の応答で、デリゲートが返されます。</span><span class="sxs-lookup"><span data-stu-id="52faa-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="52faa-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="52faa-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="52faa-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="52faa-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="52faa-108">Attributes and elements</span></span>

<span data-ttu-id="52faa-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="52faa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52faa-110">属性</span><span class="sxs-lookup"><span data-stu-id="52faa-110">Attributes</span></span>

<span data-ttu-id="52faa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="52faa-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52faa-112">子要素</span><span class="sxs-lookup"><span data-stu-id="52faa-112">Child elements</span></span>

|<span data-ttu-id="52faa-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="52faa-113">**Element**</span></span>|<span data-ttu-id="52faa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="52faa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52faa-115">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="52faa-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="52faa-116">デリゲートを識別します。</span><span class="sxs-lookup"><span data-stu-id="52faa-116">Identifies the delegate.</span></span> <span data-ttu-id="52faa-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="52faa-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="52faa-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="52faa-119">デリゲートのアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="52faa-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="52faa-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="52faa-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="52faa-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="52faa-122">代理人が会議に関連するプリンシパルにアドレス指定されたメッセージのコピーを受け取るかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="52faa-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="52faa-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="52faa-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="52faa-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="52faa-125">代理人が主体のメールボックスにプライベートの予定表アイテムを表示する権限を持つかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="52faa-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="52faa-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52faa-127">親要素</span><span class="sxs-lookup"><span data-stu-id="52faa-127">Parent elements</span></span>

|<span data-ttu-id="52faa-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="52faa-128">**Element**</span></span>|<span data-ttu-id="52faa-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="52faa-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52faa-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="52faa-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="52faa-131">追加または更新のメールボックスに代理人の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="52faa-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="52faa-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="52faa-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="52faa-133">代理人の管理操作の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="52faa-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="52faa-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="52faa-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="52faa-135">備考</span><span class="sxs-lookup"><span data-stu-id="52faa-135">Remarks</span></span>

<span data-ttu-id="52faa-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="52faa-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52faa-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="52faa-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52faa-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="52faa-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52faa-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="52faa-139">Schema Name</span></span>  <br/> |<span data-ttu-id="52faa-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="52faa-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="52faa-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="52faa-141">Validation File</span></span>  <br/> |<span data-ttu-id="52faa-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="52faa-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="52faa-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="52faa-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="52faa-144">False</span><span class="sxs-lookup"><span data-stu-id="52faa-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52faa-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="52faa-145">See also</span></span>

- [<span data-ttu-id="52faa-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="52faa-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="52faa-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="52faa-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="52faa-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="52faa-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="52faa-149">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="52faa-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


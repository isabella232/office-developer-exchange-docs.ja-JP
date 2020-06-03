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
description: DelegateUser 要素は、メールボックスまたは代理人管理応答で返された代理人に対して追加または更新する単一の代理人を指定します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458804"
---
# <a name="delegateuser"></a><span data-ttu-id="a38ea-104">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="a38ea-104">DelegateUser</span></span>

<span data-ttu-id="a38ea-105">**DelegateUser**要素は、メールボックスまたは代理人管理応答で返された代理人に対して追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="a38ea-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="a38ea-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="a38ea-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="a38ea-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a38ea-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a38ea-108">Attributes and elements</span></span>

<span data-ttu-id="a38ea-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a38ea-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a38ea-110">属性</span><span class="sxs-lookup"><span data-stu-id="a38ea-110">Attributes</span></span>

<span data-ttu-id="a38ea-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a38ea-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a38ea-112">子要素</span><span class="sxs-lookup"><span data-stu-id="a38ea-112">Child elements</span></span>

|<span data-ttu-id="a38ea-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="a38ea-113">**Element**</span></span>|<span data-ttu-id="a38ea-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a38ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a38ea-115">UserId</span><span class="sxs-lookup"><span data-stu-id="a38ea-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="a38ea-116">代理人を識別します。</span><span class="sxs-lookup"><span data-stu-id="a38ea-116">Identifies the delegate.</span></span> <span data-ttu-id="a38ea-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a38ea-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="a38ea-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="a38ea-119">代理人のアクセス許可レベルの設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a38ea-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="a38ea-120">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a38ea-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="a38ea-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="a38ea-122">代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a38ea-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="a38ea-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="a38ea-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="a38ea-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="a38ea-125">代理人が、プリンシパルのメールボックス内の個人の予定表アイテムを表示する権限を持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a38ea-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="a38ea-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a38ea-127">親要素</span><span class="sxs-lookup"><span data-stu-id="a38ea-127">Parent elements</span></span>

|<span data-ttu-id="a38ea-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="a38ea-128">**Element**</span></span>|<span data-ttu-id="a38ea-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="a38ea-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a38ea-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="a38ea-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="a38ea-131">メールボックスで追加または更新する代理人の id が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a38ea-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="a38ea-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="a38ea-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="a38ea-133">代理人管理操作の応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a38ea-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="a38ea-134">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a38ea-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a38ea-135">注釈</span><span class="sxs-lookup"><span data-stu-id="a38ea-135">Remarks</span></span>

<span data-ttu-id="a38ea-136">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a38ea-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a38ea-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a38ea-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a38ea-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="a38ea-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a38ea-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a38ea-139">Schema Name</span></span>  <br/> |<span data-ttu-id="a38ea-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a38ea-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="a38ea-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a38ea-141">Validation File</span></span>  <br/> |<span data-ttu-id="a38ea-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a38ea-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a38ea-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a38ea-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="a38ea-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="a38ea-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a38ea-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="a38ea-145">See also</span></span>

- [<span data-ttu-id="a38ea-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="a38ea-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="a38ea-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="a38ea-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="a38ea-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a38ea-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a38ea-149">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="a38ea-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


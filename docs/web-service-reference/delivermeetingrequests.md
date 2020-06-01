---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: DeliverMeetingRequests 要素は、代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463679"
---
# <a name="delivermeetingrequests"></a><span data-ttu-id="32d00-104">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="32d00-104">DeliverMeetingRequests</span></span>

<span data-ttu-id="32d00-105">**DeliverMeetingRequests**要素は、代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="32d00-105">The **DeliverMeetingRequests** element defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="32d00-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32d00-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 <span data-ttu-id="32d00-107">**DeliverMeetingRequestsType**</span><span class="sxs-lookup"><span data-stu-id="32d00-107">**DeliverMeetingRequestsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32d00-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="32d00-108">Attributes and elements</span></span>

<span data-ttu-id="32d00-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32d00-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32d00-110">属性</span><span class="sxs-lookup"><span data-stu-id="32d00-110">Attributes</span></span>

<span data-ttu-id="32d00-111">なし。</span><span class="sxs-lookup"><span data-stu-id="32d00-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32d00-112">子要素</span><span class="sxs-lookup"><span data-stu-id="32d00-112">Child elements</span></span>

<span data-ttu-id="32d00-113">なし。</span><span class="sxs-lookup"><span data-stu-id="32d00-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32d00-114">親要素</span><span class="sxs-lookup"><span data-stu-id="32d00-114">Parent elements</span></span>

|<span data-ttu-id="32d00-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="32d00-115">**Element**</span></span>|<span data-ttu-id="32d00-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d00-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32d00-117">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="32d00-117">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="32d00-118">メールボックスに代理人を追加するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="32d00-118">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="32d00-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32d00-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="32d00-120">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="32d00-120">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="32d00-121">メールボックスの代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="32d00-121">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="32d00-122">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32d00-122">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="32d00-123">GetDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="32d00-123">GetDelegateResponse</span></span>](getdelegateresponse.md) <br/> |<span data-ttu-id="32d00-124">GetDelegate 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="32d00-124">Contains the status and result of a GetDelegate request.</span></span> <span data-ttu-id="32d00-125">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="32d00-125">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32d00-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32d00-126">Text value</span></span>

<span data-ttu-id="32d00-127">次の表に、 **DeliverMeetingRequests**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="32d00-127">The following table lists the possible values for the **DeliverMeetingRequests** element.</span></span> 
  
<span data-ttu-id="32d00-128">**DeliverMeetingRequests 要素の値**</span><span class="sxs-lookup"><span data-stu-id="32d00-128">**DeliverMeetingRequests element values**</span></span>

|<span data-ttu-id="32d00-129">**値**</span><span class="sxs-lookup"><span data-stu-id="32d00-129">**Value**</span></span>|<span data-ttu-id="32d00-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="32d00-130">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32d00-131">DelegatesOnly</span><span class="sxs-lookup"><span data-stu-id="32d00-131">DelegatesOnly</span></span>  <br/> |<span data-ttu-id="32d00-132">会議出席依頼は代理人に転送され、プリンシパルのメールボックス内の [削除済みアイテム] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="32d00-132">Meeting requests are forwarded to the delegate and moved to the Deleted Items folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="32d00-133">DelegatesAndMe</span><span class="sxs-lookup"><span data-stu-id="32d00-133">DelegatesAndMe</span></span>  <br/> |<span data-ttu-id="32d00-134">会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイフォルダーに残ります。</span><span class="sxs-lookup"><span data-stu-id="32d00-134">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox.</span></span>  <br/> |
|<span data-ttu-id="32d00-135">DelegatesAndSendInformationToMe</span><span class="sxs-lookup"><span data-stu-id="32d00-135">DelegatesAndSendInformationToMe</span></span>  <br/> |<span data-ttu-id="32d00-136">会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイフォルダーに残りますが、[承諾]、[仮承諾]、[辞退] の各ボタンは、Microsoft Office Outlook の閲覧ウィンドウに表示されません。</span><span class="sxs-lookup"><span data-stu-id="32d00-136">Meeting requests are forwarded to the delegate and remain in the Inbox folder in the principal's mailbox, but the Accept, Tentative, and Decline buttons do not appear in the Microsoft Office Outlook reading pane.</span></span>  <br/> |
|<span data-ttu-id="32d00-137">NoForward</span><span class="sxs-lookup"><span data-stu-id="32d00-137">NoForward</span></span>  <br/> |<span data-ttu-id="32d00-138">会議出席依頼は代理人に転送されません。</span><span class="sxs-lookup"><span data-stu-id="32d00-138">Meeting requests are not forwarded to the delegate.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="32d00-139">注釈</span><span class="sxs-lookup"><span data-stu-id="32d00-139">Remarks</span></span>

<span data-ttu-id="32d00-140">**DeliverMeetingRequests**設定は、プリンシパルのメールボックス内のすべての代理人に影響します。</span><span class="sxs-lookup"><span data-stu-id="32d00-140">The **DeliverMeetingRequests** setting affects all delegates in a principal's mailbox.</span></span> 
  
<span data-ttu-id="32d00-141">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="32d00-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32d00-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="32d00-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32d00-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="32d00-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32d00-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32d00-144">Schema Name</span></span>  <br/> |<span data-ttu-id="32d00-145">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="32d00-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32d00-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32d00-146">Validation File</span></span>  <br/> |<span data-ttu-id="32d00-147">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="32d00-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32d00-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32d00-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="32d00-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="32d00-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32d00-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="32d00-150">See also</span></span>

- [<span data-ttu-id="32d00-151">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="32d00-151">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="32d00-152">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="32d00-152">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="32d00-153">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="32d00-153">GetDelegate operation</span></span>](getdelegate-operation.md)
- [<span data-ttu-id="32d00-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="32d00-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="32d00-155">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="32d00-155">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)


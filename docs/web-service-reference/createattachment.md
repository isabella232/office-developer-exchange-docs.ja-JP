---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: CreateAttachment 要素は、Exchange ストア内のアイテムに添付ファイルを作成するための要求を定義します。
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466438"
---
# <a name="createattachment"></a><span data-ttu-id="ae1d0-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ae1d0-103">CreateAttachment</span></span>

<span data-ttu-id="ae1d0-104">**Createattachment**要素は、Exchange ストア内のアイテムに添付ファイルを作成するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="ae1d0-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ae1d0-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae1d0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ae1d0-106">Attributes and elements</span></span>

<span data-ttu-id="ae1d0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae1d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae1d0-108">Attributes</span></span>

<span data-ttu-id="ae1d0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae1d0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ae1d0-110">Child elements</span></span>

|<span data-ttu-id="ae1d0-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ae1d0-111">**Element**</span></span>|<span data-ttu-id="ae1d0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ae1d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae1d0-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="ae1d0-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="ae1d0-114">作成された添付ファイルを含む親 Exchange ストアアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="ae1d0-115">[Parentitemid](parentitemid.md)要素は、実際の Exchange ストアアイテムの ID を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="ae1d0-116">実際のストアアイテムは、 [GetItem 操作](getitem-operation.md)を使用して取得できます。添付ファイルは、 [Getattachment 操作](getattachment-operation.md)を使用して取得されます。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="ae1d0-117">[Parentitemid](parentitemid.md)に添付ファイルの id が渡されると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="ae1d0-118">[Parentitemid](parentitemid.md)が既存のアイテムの添付ファイルの id を表す場合、 [createattachment 操作](createattachment-operation.md)は既存の添付ファイルに新しい添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="ae1d0-119">この要素は、 [Createattachment 操作](createattachment-operation.md)に必要です。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ae1d0-120">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="ae1d0-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ae1d0-121">Exchange ストア内のアイテムに添付するアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae1d0-122">親要素</span><span class="sxs-lookup"><span data-stu-id="ae1d0-122">Parent elements</span></span>

<span data-ttu-id="ae1d0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae1d0-124">注釈</span><span class="sxs-lookup"><span data-stu-id="ae1d0-124">Remarks</span></span>

<span data-ttu-id="ae1d0-125">アイテムの添付ファイルは、ストアアイテムとして存在しません。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="ae1d0-126">アイテムまたは他の添付ファイルの添付ファイルとしてのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="ae1d0-127">アイテムの添付ファイルは、 [Getattachment](getattachment.md)要求を使用してのみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="ae1d0-128">次のアイテムの添付ファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="ae1d0-129">項目</span><span class="sxs-lookup"><span data-stu-id="ae1d0-129">Item</span></span>
    
- <span data-ttu-id="ae1d0-130">メッセージ</span><span class="sxs-lookup"><span data-stu-id="ae1d0-130">Message</span></span>
    
- <span data-ttu-id="ae1d0-131">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ae1d0-131">CalendarItem</span></span>
    
- <span data-ttu-id="ae1d0-132">Contact</span><span class="sxs-lookup"><span data-stu-id="ae1d0-132">Contact</span></span>
    
- <span data-ttu-id="ae1d0-133">タスク</span><span class="sxs-lookup"><span data-stu-id="ae1d0-133">Task</span></span>
    
- <span data-ttu-id="ae1d0-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ae1d0-134">MeetingMessage</span></span>
    
- <span data-ttu-id="ae1d0-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ae1d0-135">MeetingRequest</span></span>
    
<span data-ttu-id="ae1d0-136">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ae1d0-137">例</span><span class="sxs-lookup"><span data-stu-id="ae1d0-137">Example</span></span>

<span data-ttu-id="ae1d0-138">次の例は、Exchange ストア内の別のアイテムにアイテムを作成して接続する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ae1d0-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="ae1d0-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ae1d0-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae1d0-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae1d0-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae1d0-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ae1d0-141">Schema Name</span></span>  <br/> |<span data-ttu-id="ae1d0-142">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ae1d0-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae1d0-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ae1d0-143">Validation File</span></span>  <br/> |<span data-ttu-id="ae1d0-144">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ae1d0-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae1d0-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ae1d0-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae1d0-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="ae1d0-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae1d0-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="ae1d0-147">See also</span></span>



[<span data-ttu-id="ae1d0-148">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="ae1d0-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="ae1d0-149">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="ae1d0-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="ae1d0-150">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="ae1d0-150">GetAttachment operation</span></span>](getattachment-operation.md)


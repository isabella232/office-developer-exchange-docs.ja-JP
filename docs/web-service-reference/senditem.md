---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: SendItem 要素は、Exchange ストア内のアイテムを送信するための要求のルート要素です。
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530566"
---
# <a name="senditem"></a><span data-ttu-id="2d7ee-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="2d7ee-103">SendItem</span></span>

<span data-ttu-id="2d7ee-104">**SendItem**要素は、Exchange ストア内のアイテムを送信するための要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="2d7ee-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d7ee-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2d7ee-106">Attributes and elements</span></span>

<span data-ttu-id="2d7ee-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d7ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d7ee-108">Attributes</span></span>

|<span data-ttu-id="2d7ee-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-109">**Attribute**</span></span>|<span data-ttu-id="2d7ee-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2d7ee-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="2d7ee-112">送信されたアイテムのコピーを保存するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="2d7ee-113">Save アクションは、 **Saveitemtofolder**の値と、要求に[SavedItemFolderId](saveditemfolderid.md)要素が存在するかどうかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="2d7ee-114">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="2d7ee-115">SaveItemToFolder 属性</span><span class="sxs-lookup"><span data-stu-id="2d7ee-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="2d7ee-116">**値**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-116">**Value**</span></span>|<span data-ttu-id="2d7ee-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2d7ee-118">**true**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-118">**true**</span></span> <br/> |<span data-ttu-id="2d7ee-119">[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="2d7ee-120">[SavedItemFolderId](saveditemfolderid.md)要素が存在する場合は、 [SavedItemFolderId](saveditemfolderid.md)要素によって指定されたフォルダーにアイテムが保存されます。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="2d7ee-121">**false**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-121">**false**</span></span> <br/> |<span data-ttu-id="2d7ee-122">[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合、アイテムは保存されません。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="2d7ee-123">[SavedItemFolderId](saveditemfolderid.md)要素が存在する場合は、エラー応答が返されます。この値は、 **Errorinvalidsenditemsavesettings**値を[含む、応答](responsecode.md)します。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2d7ee-124">子要素</span><span class="sxs-lookup"><span data-stu-id="2d7ee-124">Child elements</span></span>

|<span data-ttu-id="2d7ee-125">**Element**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-125">**Element**</span></span>|<span data-ttu-id="2d7ee-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d7ee-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d7ee-127">ItemIds</span><span class="sxs-lookup"><span data-stu-id="2d7ee-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="2d7ee-128">Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用されるアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d7ee-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="2d7ee-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="2d7ee-130">Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d7ee-131">親要素</span><span class="sxs-lookup"><span data-stu-id="2d7ee-131">Parent elements</span></span>

<span data-ttu-id="2d7ee-132">なし。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2d7ee-133">注釈</span><span class="sxs-lookup"><span data-stu-id="2d7ee-133">Remarks</span></span>

<span data-ttu-id="2d7ee-134">送信済みアイテムフォルダー内のアイテムが送信されると、送信されたアイテムは削除され、そのコピーが [送信済みアイテム] フォルダーに配置されます。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="2d7ee-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2d7ee-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d7ee-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2d7ee-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d7ee-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="2d7ee-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d7ee-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d7ee-138">Schema Name</span></span>  <br/> |<span data-ttu-id="2d7ee-139">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2d7ee-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d7ee-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d7ee-140">Validation File</span></span>  <br/> |<span data-ttu-id="2d7ee-141">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2d7ee-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d7ee-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2d7ee-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d7ee-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="2d7ee-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d7ee-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d7ee-144">See also</span></span>



[<span data-ttu-id="2d7ee-145">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="2d7ee-145">SendItem operation</span></span>](senditem-operation.md)


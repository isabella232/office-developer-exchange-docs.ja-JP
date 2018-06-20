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
description: SendItem 要素は、Exchange ストア内のアイテムを送信する要求のルート要素です。
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833340"
---
# <a name="senditem"></a><span data-ttu-id="faf8b-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="faf8b-103">SendItem</span></span>

<span data-ttu-id="faf8b-104">**SendItem**要素は、Exchange ストア内のアイテムを送信する要求のルート要素です。</span><span class="sxs-lookup"><span data-stu-id="faf8b-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="faf8b-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="faf8b-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faf8b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="faf8b-106">Attributes and elements</span></span>

<span data-ttu-id="faf8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faf8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="faf8b-108">Attributes</span></span>

|<span data-ttu-id="faf8b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="faf8b-109">**Attribute**</span></span>|<span data-ttu-id="faf8b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf8b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="faf8b-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="faf8b-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="faf8b-112">送信済みアイテムのコピーを保存するかどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="faf8b-113">保存アクションは、 **SaveItemToFolder**と[SavedItemFolderId](saveditemfolderid.md)要素が要求内に存在するかどうかの値によって異なります。</span><span class="sxs-lookup"><span data-stu-id="faf8b-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="faf8b-114">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="faf8b-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="faf8b-115">SaveItemToFolder 属性</span><span class="sxs-lookup"><span data-stu-id="faf8b-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="faf8b-116">**値**</span><span class="sxs-lookup"><span data-stu-id="faf8b-116">**Value**</span></span>|<span data-ttu-id="faf8b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf8b-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="faf8b-118">**true**</span><span class="sxs-lookup"><span data-stu-id="faf8b-118">**true**</span></span> <br/> |<span data-ttu-id="faf8b-119">[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合は、送信済みアイテム フォルダーにアイテムを保存します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="faf8b-120">[SavedItemFolderId](saveditemfolderid.md)要素が存在する場合、 [SavedItemFolderId](saveditemfolderid.md)要素で指定されているフォルダーにアイテムを保存します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="faf8b-121">**false**</span><span class="sxs-lookup"><span data-stu-id="faf8b-121">**false**</span></span> <br/> |<span data-ttu-id="faf8b-122">[SavedItemFolderId](saveditemfolderid.md)要素が存在しない場合は、アイテムは保存されません。</span><span class="sxs-lookup"><span data-stu-id="faf8b-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="faf8b-123">[SavedItemFolderId](saveditemfolderid.md)要素が存在する場合、 **ErrorInvalidSendItemSaveSettings**値を格納する[ResponseCode](responsecode.md)要素を使用して、エラー応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="faf8b-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="faf8b-124">子要素</span><span class="sxs-lookup"><span data-stu-id="faf8b-124">Child elements</span></span>

|<span data-ttu-id="faf8b-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="faf8b-125">**Element**</span></span>|<span data-ttu-id="faf8b-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf8b-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faf8b-127">Itemid</span><span class="sxs-lookup"><span data-stu-id="faf8b-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="faf8b-128">アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムのコピーに使用される、マスターの定期的なアイテムの一意の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faf8b-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="faf8b-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="faf8b-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="faf8b-130">更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="faf8b-131">親要素</span><span class="sxs-lookup"><span data-stu-id="faf8b-131">Parent elements</span></span>

<span data-ttu-id="faf8b-132">なし。</span><span class="sxs-lookup"><span data-stu-id="faf8b-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="faf8b-133">備考</span><span class="sxs-lookup"><span data-stu-id="faf8b-133">Remarks</span></span>

<span data-ttu-id="faf8b-134">送信済みアイテム フォルダー内のアイテムが送信された場合、送信済みアイテムを削除しのコピーが送信済みアイテム フォルダーに配置します。</span><span class="sxs-lookup"><span data-stu-id="faf8b-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="faf8b-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="faf8b-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faf8b-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="faf8b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faf8b-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="faf8b-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="faf8b-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="faf8b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="faf8b-139">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="faf8b-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="faf8b-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="faf8b-140">Validation File</span></span>  <br/> |<span data-ttu-id="faf8b-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="faf8b-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="faf8b-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="faf8b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="faf8b-143">False</span><span class="sxs-lookup"><span data-stu-id="faf8b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="faf8b-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="faf8b-144">See also</span></span>



<span data-ttu-id="faf8b-145">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="faf8b-145">[SendItem operation](senditem-operation.md)</span></span>


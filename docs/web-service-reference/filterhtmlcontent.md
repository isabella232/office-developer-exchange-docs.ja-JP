---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: FilterHtmlContent 要素は、安全でない可能性のある HTML コンテンツをアイテムまたは添付ファイルからフィルター処理するかどうかを指定します。
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462676"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="cb956-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="cb956-103">FilterHtmlContent</span></span>

<span data-ttu-id="cb956-104">**Filterhtmlcontent**要素は、安全でない可能性のある HTML コンテンツをアイテムまたは添付ファイルからフィルター処理するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb956-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="cb956-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="cb956-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb956-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cb956-106">Attributes and elements</span></span>

<span data-ttu-id="cb956-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb956-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb956-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb956-108">Attributes</span></span>

<span data-ttu-id="cb956-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cb956-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb956-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cb956-110">Child elements</span></span>

<span data-ttu-id="cb956-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cb956-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb956-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cb956-112">Parent elements</span></span>

|<span data-ttu-id="cb956-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb956-113">**Element**</span></span>|<span data-ttu-id="cb956-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb956-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb956-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="cb956-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="cb956-116">[Getattachment](getattachment.md)要求に対する応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="cb956-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="cb956-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb956-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="cb956-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="cb956-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="cb956-119">GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="cb956-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="cb956-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cb956-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb956-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cb956-121">Text value</span></span>

<span data-ttu-id="cb956-122">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="cb956-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="cb956-123">既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="cb956-123">The default value is **false**.</span></span> <span data-ttu-id="cb956-124">これは Boolean データ型です。</span><span class="sxs-lookup"><span data-stu-id="cb956-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cb956-125">注釈</span><span class="sxs-lookup"><span data-stu-id="cb956-125">Remarks</span></span>

<span data-ttu-id="cb956-126">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="cb956-126">This element is optional.</span></span>
  
<span data-ttu-id="cb956-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cb956-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb956-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cb956-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb956-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb956-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb956-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cb956-130">Schema Name</span></span>  <br/> |<span data-ttu-id="cb956-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cb956-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb956-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cb956-132">Validation File</span></span>  <br/> |<span data-ttu-id="cb956-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cb956-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb956-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cb956-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb956-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="cb956-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb956-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb956-136">See also</span></span>

- [<span data-ttu-id="cb956-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb956-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


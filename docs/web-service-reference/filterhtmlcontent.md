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
description: FilterHtmlContent 要素は、アイテムまたは添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。
ms.openlocfilehash: db181eff9586061d728a5e4ef55a78f4955b5713
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760485"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="e007c-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="e007c-103">FilterHtmlContent</span></span>

<span data-ttu-id="e007c-104">**FilterHtmlContent**要素は、アイテムまたは添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e007c-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="e007c-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e007c-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e007c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e007c-106">Attributes and elements</span></span>

<span data-ttu-id="e007c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e007c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e007c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e007c-108">Attributes</span></span>

<span data-ttu-id="e007c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e007c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e007c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e007c-110">Child elements</span></span>

<span data-ttu-id="e007c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e007c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e007c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e007c-112">Parent elements</span></span>

|<span data-ttu-id="e007c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e007c-113">**Element**</span></span>|<span data-ttu-id="e007c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e007c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e007c-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="e007c-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="e007c-116">[GetAttachment](getattachment.md)要求への応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e007c-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="e007c-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e007c-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="e007c-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e007c-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="e007c-119">GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e007c-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="e007c-120">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="e007c-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e007c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e007c-121">Text value</span></span>

<span data-ttu-id="e007c-122">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="e007c-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="e007c-123">既定値は、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="e007c-123">The default value is **false**.</span></span> <span data-ttu-id="e007c-124">これは、ブール型のデータ型です。</span><span class="sxs-lookup"><span data-stu-id="e007c-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e007c-125">備考</span><span class="sxs-lookup"><span data-stu-id="e007c-125">Remarks</span></span>

<span data-ttu-id="e007c-126">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="e007c-126">This element is optional.</span></span>
  
<span data-ttu-id="e007c-127">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e007c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e007c-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="e007c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e007c-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="e007c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e007c-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e007c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e007c-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e007c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="e007c-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e007c-132">Validation File</span></span>  <br/> |<span data-ttu-id="e007c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e007c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e007c-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e007c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e007c-135">False</span><span class="sxs-lookup"><span data-stu-id="e007c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e007c-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e007c-136">See also</span></span>

- [<span data-ttu-id="e007c-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e007c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


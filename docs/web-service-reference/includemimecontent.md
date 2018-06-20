---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: IncludeMimeContent 要素は、応答で、多目的インターネット メール拡張 (MIME) のコンテンツ アイテムまたは添付ファイルが返されるかどうかを指定します。
ms.openlocfilehash: ddd6988be93231ac7c574a2e19c9ba4b562c7d0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831903"
---
# <a name="includemimecontent"></a><span data-ttu-id="8f57f-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="8f57f-103">IncludeMimeContent</span></span>

<span data-ttu-id="8f57f-104">**IncludeMimeContent**要素は、応答で、多目的インターネット メール拡張 (MIME) のコンテンツ アイテムまたは添付ファイルが返されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="8f57f-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8f57f-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f57f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8f57f-106">Attributes and elements</span></span>

<span data-ttu-id="8f57f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f57f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f57f-108">Attributes</span></span>

<span data-ttu-id="8f57f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8f57f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f57f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8f57f-110">Child elements</span></span>

<span data-ttu-id="8f57f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8f57f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8f57f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8f57f-112">Parent elements</span></span>

|<span data-ttu-id="8f57f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f57f-113">**Element**</span></span>|<span data-ttu-id="8f57f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f57f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f57f-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="8f57f-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="8f57f-116">[GetAttachment](getattachment.md)要求への応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="8f57f-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8f57f-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="8f57f-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="8f57f-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="8f57f-119">GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="8f57f-120">この要素への XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="8f57f-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f57f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8f57f-121">Text value</span></span>

<span data-ttu-id="8f57f-122">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="8f57f-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="8f57f-123">既定値は、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-123">The default value is **false**.</span></span> <span data-ttu-id="8f57f-124">これは、ブール型のデータ型です。</span><span class="sxs-lookup"><span data-stu-id="8f57f-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8f57f-125">備考</span><span class="sxs-lookup"><span data-stu-id="8f57f-125">Remarks</span></span>

<span data-ttu-id="8f57f-126">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="8f57f-126">This element is optional.</span></span>
  
<span data-ttu-id="8f57f-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8f57f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="8f57f-128">例</span><span class="sxs-lookup"><span data-stu-id="8f57f-128">Example</span></span>

<span data-ttu-id="8f57f-129">要求の例を次に示します**IncludeMimeContent**要素を設定します。</span><span class="sxs-lookup"><span data-stu-id="8f57f-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8f57f-130">添付ファイルの Id 属性は、読みやすさを保持するために切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="8f57f-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f57f-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="8f57f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f57f-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="8f57f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f57f-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f57f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8f57f-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8f57f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f57f-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f57f-135">Validation File</span></span>  <br/> |<span data-ttu-id="8f57f-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f57f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f57f-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8f57f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f57f-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="8f57f-138">False</span></span>  <br/> |
   


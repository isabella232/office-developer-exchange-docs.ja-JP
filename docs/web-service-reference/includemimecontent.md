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
description: IncludeMimeContent 要素は、アイテムまたは添付ファイルのマルチパーパスインターネットメール内線 (MIME) コンテンツが応答で返されるかどうかを指定します。
ms.openlocfilehash: 6198e4bef2dc59e6e56a8d3cbe463dad13e544e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457194"
---
# <a name="includemimecontent"></a><span data-ttu-id="6610a-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="6610a-103">IncludeMimeContent</span></span>

<span data-ttu-id="6610a-104">**IncludeMimeContent**要素は、アイテムまたは添付ファイルのマルチパーパスインターネットメール内線 (MIME) コンテンツが応答で返されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6610a-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="6610a-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="6610a-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6610a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6610a-106">Attributes and elements</span></span>

<span data-ttu-id="6610a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6610a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6610a-108">属性</span><span class="sxs-lookup"><span data-stu-id="6610a-108">Attributes</span></span>

<span data-ttu-id="6610a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6610a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6610a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6610a-110">Child elements</span></span>

<span data-ttu-id="6610a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6610a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6610a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6610a-112">Parent elements</span></span>

|<span data-ttu-id="6610a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6610a-113">**Element**</span></span>|<span data-ttu-id="6610a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6610a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6610a-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="6610a-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="6610a-116">[Getattachment](getattachment.md)要求に対する応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6610a-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="6610a-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6610a-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="6610a-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="6610a-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="6610a-119">GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="6610a-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="6610a-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6610a-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6610a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6610a-121">Text value</span></span>

<span data-ttu-id="6610a-122">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="6610a-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="6610a-123">既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="6610a-123">The default value is **false**.</span></span> <span data-ttu-id="6610a-124">これは Boolean データ型です。</span><span class="sxs-lookup"><span data-stu-id="6610a-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6610a-125">注釈</span><span class="sxs-lookup"><span data-stu-id="6610a-125">Remarks</span></span>

<span data-ttu-id="6610a-126">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="6610a-126">This element is optional.</span></span>
  
<span data-ttu-id="6610a-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6610a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6610a-128">例</span><span class="sxs-lookup"><span data-stu-id="6610a-128">Example</span></span>

<span data-ttu-id="6610a-129">次の要求例は、 **IncludeMimeContent**要素の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6610a-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="6610a-130">添付ファイル Id 属性は、読みやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="6610a-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6610a-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6610a-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6610a-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="6610a-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6610a-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6610a-133">Schema Name</span></span>  <br/> |<span data-ttu-id="6610a-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6610a-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="6610a-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6610a-135">Validation File</span></span>  <br/> |<span data-ttu-id="6610a-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6610a-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6610a-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6610a-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="6610a-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="6610a-138">False</span></span>  <br/> |
   


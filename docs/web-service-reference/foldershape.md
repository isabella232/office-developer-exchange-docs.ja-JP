---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: FolderShape 要素は、GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを指定します。
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461346"
---
# <a name="foldershape"></a><span data-ttu-id="74b3c-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="74b3c-103">FolderShape</span></span>

<span data-ttu-id="74b3c-104">**Foldershape**要素は、 [getfolder](getfolder.md)、 [Findfolder](findfolder.md)、または[syncfolderhierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="74b3c-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="74b3c-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74b3c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74b3c-106">Attributes and elements</span></span>

<span data-ttu-id="74b3c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74b3c-108">属性</span><span class="sxs-lookup"><span data-stu-id="74b3c-108">Attributes</span></span>

<span data-ttu-id="74b3c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74b3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74b3c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74b3c-110">Child elements</span></span>

|<span data-ttu-id="74b3c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="74b3c-111">**Element**</span></span>|<span data-ttu-id="74b3c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74b3c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74b3c-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="74b3c-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="74b3c-114">応答で返されるプロパティの基本的な構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="74b3c-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="74b3c-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="74b3c-116">応答で返される追加のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74b3c-117">親要素</span><span class="sxs-lookup"><span data-stu-id="74b3c-117">Parent elements</span></span>

|<span data-ttu-id="74b3c-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="74b3c-118">**Element**</span></span>|<span data-ttu-id="74b3c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="74b3c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74b3c-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="74b3c-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="74b3c-121">メールボックス内のフォルダーを識別する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="74b3c-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="74b3c-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="74b3c-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="74b3c-124">Exchange ストアからフォルダーを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="74b3c-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="74b3c-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="74b3c-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="74b3c-127">クライアント上のフォルダー階層を同期する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="74b3c-128">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74b3c-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74b3c-129">注釈</span><span class="sxs-lookup"><span data-stu-id="74b3c-129">Remarks</span></span>

<span data-ttu-id="74b3c-130">**Foldershape**要素は、 [findfolder](findfolder.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="74b3c-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="74b3c-131">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="74b3c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="74b3c-132">例</span><span class="sxs-lookup"><span data-stu-id="74b3c-132">Example</span></span>

<span data-ttu-id="74b3c-133">次の要求例は、受信トレイフォルダーの最初のレベルにあるすべてのフォルダーを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="74b3c-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="74b3c-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74b3c-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74b3c-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="74b3c-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74b3c-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74b3c-136">Schema Name</span></span>  <br/> |<span data-ttu-id="74b3c-137">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="74b3c-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74b3c-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74b3c-138">Validation File</span></span>  <br/> |<span data-ttu-id="74b3c-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="74b3c-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74b3c-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74b3c-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="74b3c-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="74b3c-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74b3c-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="74b3c-142">See also</span></span>



[<span data-ttu-id="74b3c-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="74b3c-143">FindFolder</span></span>](findfolder.md)


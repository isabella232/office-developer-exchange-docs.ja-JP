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
description: FolderShape 要素は、GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760582"
---
# <a name="foldershape"></a><span data-ttu-id="05765-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="05765-103">FolderShape</span></span>

<span data-ttu-id="05765-104">**FolderShape**要素は、 [GetFolder](getfolder.md)、 [FindFolder](findfolder.md)、または[SyncFolderHierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="05765-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="05765-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="05765-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05765-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="05765-106">Attributes and elements</span></span>

<span data-ttu-id="05765-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05765-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05765-108">属性</span><span class="sxs-lookup"><span data-stu-id="05765-108">Attributes</span></span>

<span data-ttu-id="05765-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05765-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05765-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05765-110">Child elements</span></span>

|<span data-ttu-id="05765-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="05765-111">**Element**</span></span>|<span data-ttu-id="05765-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="05765-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05765-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="05765-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="05765-114">応答で返されるプロパティの基本構成を識別します。</span><span class="sxs-lookup"><span data-stu-id="05765-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="05765-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="05765-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="05765-116">応答で返される追加プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="05765-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05765-117">親要素</span><span class="sxs-lookup"><span data-stu-id="05765-117">Parent elements</span></span>

|<span data-ttu-id="05765-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="05765-118">**Element**</span></span>|<span data-ttu-id="05765-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="05765-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05765-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="05765-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="05765-121">メールボックス内のフォルダーを識別するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="05765-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="05765-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="05765-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="05765-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="05765-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="05765-124">Exchange ストアからフォルダーを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="05765-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="05765-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="05765-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="05765-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="05765-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="05765-127">クライアント上のフォルダー階層を同期するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="05765-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="05765-128">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="05765-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05765-129">備考</span><span class="sxs-lookup"><span data-stu-id="05765-129">Remarks</span></span>

<span data-ttu-id="05765-130">**FolderShape**要素は、 [FindFolder](findfolder.md)要素の必須の子要素です。</span><span class="sxs-lookup"><span data-stu-id="05765-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="05765-131">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="05765-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="05765-132">例</span><span class="sxs-lookup"><span data-stu-id="05765-132">Example</span></span>

<span data-ttu-id="05765-133">要求の次の例では、[受信トレイ] フォルダーの最初のレベルにあるすべてのフォルダーを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="05765-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="05765-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="05765-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05765-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="05765-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="05765-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05765-136">Schema Name</span></span>  <br/> |<span data-ttu-id="05765-137">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="05765-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="05765-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05765-138">Validation File</span></span>  <br/> |<span data-ttu-id="05765-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="05765-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05765-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="05765-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="05765-141">False</span><span class="sxs-lookup"><span data-stu-id="05765-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05765-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="05765-142">See also</span></span>



[<span data-ttu-id="05765-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="05765-143">FindFolder</span></span>](findfolder.md)


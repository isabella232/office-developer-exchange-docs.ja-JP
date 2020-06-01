---
title: FileAsMapping
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAsMapping
api_type:
- schema
ms.assetid: 2c98e7c6-09b0-47b3-bbf7-8c4ef9510280
description: FileAsMapping 要素は、連絡先に対して表示される内容を作成する方法を定義します。
ms.openlocfilehash: d846c0af0fbad4df9ee800fe136a4ffcc74c8608
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461038"
---
# <a name="fileasmapping"></a><span data-ttu-id="b6524-103">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="b6524-103">FileAsMapping</span></span>

<span data-ttu-id="b6524-104">**Fileasmapping**要素は、連絡先に対して表示される内容を作成する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="b6524-104">The **FileAsMapping** element defines how to construct what is displayed for a contact.</span></span> 
  
```xml
<FileAsMapping/>
```

 <span data-ttu-id="b6524-105">**FileAsMappingType**</span><span class="sxs-lookup"><span data-stu-id="b6524-105">**FileAsMappingType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6524-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6524-106">Attributes and elements</span></span>

<span data-ttu-id="b6524-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6524-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6524-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6524-108">Attributes</span></span>

<span data-ttu-id="b6524-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6524-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6524-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6524-110">Child elements</span></span>

<span data-ttu-id="b6524-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b6524-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6524-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6524-112">Parent elements</span></span>

|<span data-ttu-id="b6524-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6524-113">**Element**</span></span>|<span data-ttu-id="b6524-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6524-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6524-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="b6524-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b6524-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b6524-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b6524-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b6524-117">Text value</span></span>

<span data-ttu-id="b6524-118">この要素のテキスト値は、次のいずれかの文字列値に制限されています。</span><span class="sxs-lookup"><span data-stu-id="b6524-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="b6524-119">なし</span><span class="sxs-lookup"><span data-stu-id="b6524-119">None</span></span>
    
- <span data-ttu-id="b6524-120">LastCommaFirst</span><span class="sxs-lookup"><span data-stu-id="b6524-120">LastCommaFirst</span></span>
    
- <span data-ttu-id="b6524-121">FirstSpaceLast</span><span class="sxs-lookup"><span data-stu-id="b6524-121">FirstSpaceLast</span></span>
    
- <span data-ttu-id="b6524-122">Company</span><span class="sxs-lookup"><span data-stu-id="b6524-122">Company</span></span>
    
- <span data-ttu-id="b6524-123">LastCommaFirstCompany</span><span class="sxs-lookup"><span data-stu-id="b6524-123">LastCommaFirstCompany</span></span>
    
- <span data-ttu-id="b6524-124">CompanyLastFirst</span><span class="sxs-lookup"><span data-stu-id="b6524-124">CompanyLastFirst</span></span>
    
- <span data-ttu-id="b6524-125">LastFirst</span><span class="sxs-lookup"><span data-stu-id="b6524-125">LastFirst</span></span>
    
- <span data-ttu-id="b6524-126">LastFirstCompany</span><span class="sxs-lookup"><span data-stu-id="b6524-126">LastFirstCompany</span></span>
    
- <span data-ttu-id="b6524-127">会社の Lastcommafirst</span><span class="sxs-lookup"><span data-stu-id="b6524-127">CompanyLastCommaFirst</span></span>
    
- <span data-ttu-id="b6524-128">LastFirstSuffix</span><span class="sxs-lookup"><span data-stu-id="b6524-128">LastFirstSuffix</span></span>
    
- <span data-ttu-id="b6524-129">Lastspace Firstcompany</span><span class="sxs-lookup"><span data-stu-id="b6524-129">LastSpaceFirstCompany</span></span>
    
- <span data-ttu-id="b6524-130">会社の最終スペース</span><span class="sxs-lookup"><span data-stu-id="b6524-130">CompanyLastSpaceFirst</span></span>
    
- <span data-ttu-id="b6524-131">Lastspace の先頭</span><span class="sxs-lookup"><span data-stu-id="b6524-131">LastSpaceFirst</span></span>
    
- <span data-ttu-id="b6524-132">DisplayName</span><span class="sxs-lookup"><span data-stu-id="b6524-132">DisplayName</span></span>
    
- <span data-ttu-id="b6524-133">FirstName</span><span class="sxs-lookup"><span data-stu-id="b6524-133">FirstName</span></span>
    
- <span data-ttu-id="b6524-134">LastFirstMiddleSuffix</span><span class="sxs-lookup"><span data-stu-id="b6524-134">LastFirstMiddleSuffix</span></span>
    
- <span data-ttu-id="b6524-135">LastName</span><span class="sxs-lookup"><span data-stu-id="b6524-135">LastName</span></span>
    
- <span data-ttu-id="b6524-136">Empty</span><span class="sxs-lookup"><span data-stu-id="b6524-136">Empty</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b6524-137">注釈</span><span class="sxs-lookup"><span data-stu-id="b6524-137">Remarks</span></span>

<span data-ttu-id="b6524-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b6524-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6524-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6524-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6524-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6524-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6524-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6524-141">Schema name</span></span>  <br/> |<span data-ttu-id="b6524-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6524-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6524-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6524-143">Validation file</span></span>  <br/> |<span data-ttu-id="b6524-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b6524-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6524-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6524-145">Can be empty</span></span>  <br/> |<span data-ttu-id="b6524-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="b6524-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6524-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6524-147">See also</span></span>



- [<span data-ttu-id="b6524-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b6524-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b6524-149">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="b6524-149">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="b6524-150">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="b6524-150">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="b6524-151">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="b6524-151">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


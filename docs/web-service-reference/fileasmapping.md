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
description: FileAsMapping 要素は、連絡先の表示内容を構築する方法を定義します。
ms.openlocfilehash: 1ba0ae0daa56a72c29d8c0ccad64e3edae5f0b84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760486"
---
# <a name="fileasmapping"></a><span data-ttu-id="0a3a5-103">FileAsMapping</span><span class="sxs-lookup"><span data-stu-id="0a3a5-103">FileAsMapping</span></span>

<span data-ttu-id="0a3a5-104">**FileAsMapping**要素は、連絡先の表示内容を構築する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-104">The **FileAsMapping** element defines how to construct what is displayed for a contact.</span></span> 
  
```xml
<FileAsMapping/>
```

 <span data-ttu-id="0a3a5-105">**FileAsMappingType**</span><span class="sxs-lookup"><span data-stu-id="0a3a5-105">**FileAsMappingType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a3a5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0a3a5-106">Attributes and elements</span></span>

<span data-ttu-id="0a3a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a3a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a3a5-108">Attributes</span></span>

<span data-ttu-id="0a3a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a3a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0a3a5-110">Child elements</span></span>

<span data-ttu-id="0a3a5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a3a5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0a3a5-112">Parent elements</span></span>

|<span data-ttu-id="0a3a5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0a3a5-113">**Element**</span></span>|<span data-ttu-id="0a3a5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a3a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a3a5-115">Contact</span><span class="sxs-lookup"><span data-stu-id="0a3a5-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0a3a5-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a3a5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0a3a5-117">Text value</span></span>

<span data-ttu-id="0a3a5-118">この要素のテキスト値は、次の文字列値の 1 つに制限されています。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="0a3a5-119">なし</span><span class="sxs-lookup"><span data-stu-id="0a3a5-119">None</span></span>
    
- <span data-ttu-id="0a3a5-120">LastCommaFirst</span><span class="sxs-lookup"><span data-stu-id="0a3a5-120">LastCommaFirst</span></span>
    
- <span data-ttu-id="0a3a5-121">FirstSpaceLast</span><span class="sxs-lookup"><span data-stu-id="0a3a5-121">FirstSpaceLast</span></span>
    
- <span data-ttu-id="0a3a5-122">会社</span><span class="sxs-lookup"><span data-stu-id="0a3a5-122">Company</span></span>
    
- <span data-ttu-id="0a3a5-123">LastCommaFirstCompany</span><span class="sxs-lookup"><span data-stu-id="0a3a5-123">LastCommaFirstCompany</span></span>
    
- <span data-ttu-id="0a3a5-124">CompanyLastFirst</span><span class="sxs-lookup"><span data-stu-id="0a3a5-124">CompanyLastFirst</span></span>
    
- <span data-ttu-id="0a3a5-125">姓名</span><span class="sxs-lookup"><span data-stu-id="0a3a5-125">LastFirst</span></span>
    
- <span data-ttu-id="0a3a5-126">LastFirstCompany</span><span class="sxs-lookup"><span data-stu-id="0a3a5-126">LastFirstCompany</span></span>
    
- <span data-ttu-id="0a3a5-127">CompanyLastCommaFirst</span><span class="sxs-lookup"><span data-stu-id="0a3a5-127">CompanyLastCommaFirst</span></span>
    
- <span data-ttu-id="0a3a5-128">LastFirstSuffix</span><span class="sxs-lookup"><span data-stu-id="0a3a5-128">LastFirstSuffix</span></span>
    
- <span data-ttu-id="0a3a5-129">LastSpaceFirstCompany</span><span class="sxs-lookup"><span data-stu-id="0a3a5-129">LastSpaceFirstCompany</span></span>
    
- <span data-ttu-id="0a3a5-130">CompanyLastSpaceFirst</span><span class="sxs-lookup"><span data-stu-id="0a3a5-130">CompanyLastSpaceFirst</span></span>
    
- <span data-ttu-id="0a3a5-131">LastSpaceFirst</span><span class="sxs-lookup"><span data-stu-id="0a3a5-131">LastSpaceFirst</span></span>
    
- <span data-ttu-id="0a3a5-132">DisplayName</span><span class="sxs-lookup"><span data-stu-id="0a3a5-132">DisplayName</span></span>
    
- <span data-ttu-id="0a3a5-133">FirstName</span><span class="sxs-lookup"><span data-stu-id="0a3a5-133">FirstName</span></span>
    
- <span data-ttu-id="0a3a5-134">LastFirstMiddleSuffix</span><span class="sxs-lookup"><span data-stu-id="0a3a5-134">LastFirstMiddleSuffix</span></span>
    
- <span data-ttu-id="0a3a5-135">LastName</span><span class="sxs-lookup"><span data-stu-id="0a3a5-135">LastName</span></span>
    
- <span data-ttu-id="0a3a5-136">Empty</span><span class="sxs-lookup"><span data-stu-id="0a3a5-136">Empty</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0a3a5-137">備考</span><span class="sxs-lookup"><span data-stu-id="0a3a5-137">Remarks</span></span>

<span data-ttu-id="0a3a5-138">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a3a5-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="0a3a5-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a3a5-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="0a3a5-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a3a5-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a3a5-141">Schema name</span></span>  <br/> |<span data-ttu-id="0a3a5-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0a3a5-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a3a5-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a3a5-143">Validation file</span></span>  <br/> |<span data-ttu-id="0a3a5-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0a3a5-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a3a5-145">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-145">Can be empty</span></span>  <br/> |<span data-ttu-id="0a3a5-146">False</span><span class="sxs-lookup"><span data-stu-id="0a3a5-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a3a5-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="0a3a5-147">See also</span></span>



- [<span data-ttu-id="0a3a5-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0a3a5-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0a3a5-149">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-149">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="0a3a5-150">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="0a3a5-150">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="0a3a5-151">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="0a3a5-151">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: MSExchangeCertificate 要素には、連絡先の [Microsoft Exchange 証明書をエンコードする値が含まれています。
ms.openlocfilehash: 8d07198012485b5c6d22e1fb4721890bf9a5eb39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832498"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="18c5e-103">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="18c5e-103">MSExchangeCertificate</span></span>

<span data-ttu-id="18c5e-104">**MSExchangeCertificate**要素には、連絡先の [Microsoft Exchange 証明書をエンコードする値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="18c5e-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="18c5e-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="18c5e-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18c5e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18c5e-106">Attributes and elements</span></span>

<span data-ttu-id="18c5e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18c5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18c5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="18c5e-108">Attributes</span></span>

<span data-ttu-id="18c5e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18c5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18c5e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18c5e-110">Child elements</span></span>

|<span data-ttu-id="18c5e-111">**要素名**</span><span class="sxs-lookup"><span data-stu-id="18c5e-111">**Element name**</span></span>|<span data-ttu-id="18c5e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="18c5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18c5e-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="18c5e-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="18c5e-114">Base64 でエンコードされた値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="18c5e-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18c5e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="18c5e-115">Parent elements</span></span>

|<span data-ttu-id="18c5e-116">**要素名**</span><span class="sxs-lookup"><span data-stu-id="18c5e-116">**Element name**</span></span>|<span data-ttu-id="18c5e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="18c5e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18c5e-118">Contact</span><span class="sxs-lookup"><span data-stu-id="18c5e-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="18c5e-119">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="18c5e-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18c5e-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18c5e-120">Text value</span></span>

<span data-ttu-id="18c5e-121">なし。</span><span class="sxs-lookup"><span data-stu-id="18c5e-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18c5e-122">備考</span><span class="sxs-lookup"><span data-stu-id="18c5e-122">Remarks</span></span>

<span data-ttu-id="18c5e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18c5e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="18c5e-124">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="18c5e-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18c5e-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="18c5e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18c5e-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="18c5e-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18c5e-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18c5e-127">Schema name</span></span>  <br/> |<span data-ttu-id="18c5e-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="18c5e-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="18c5e-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18c5e-129">Validation file</span></span>  <br/> |<span data-ttu-id="18c5e-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18c5e-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18c5e-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="18c5e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="18c5e-132">False</span><span class="sxs-lookup"><span data-stu-id="18c5e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18c5e-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="18c5e-133">See also</span></span>



- [<span data-ttu-id="18c5e-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18c5e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="18c5e-135">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="18c5e-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)


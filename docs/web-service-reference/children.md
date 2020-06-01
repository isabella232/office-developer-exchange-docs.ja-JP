---
title: 子供
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Children
api_type:
- schema
ms.assetid: ceaffddd-f9bc-43ea-b348-a20fdade738f
description: 子要素には、連絡先の子の名前が含まれています。
ms.openlocfilehash: de398c93590a4a9ae93b6aa46994c9295d051b84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460226"
---
# <a name="children"></a><span data-ttu-id="a9337-103">子供</span><span class="sxs-lookup"><span data-stu-id="a9337-103">Children</span></span>

<span data-ttu-id="a9337-104">**子**要素には、連絡先の子の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9337-104">The **Children** element contains the names of a contact's children.</span></span> 
  
```xml
<Children>
   <String/>
</Children>
```

 <span data-ttu-id="a9337-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="a9337-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9337-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a9337-106">Attributes and elements</span></span>

<span data-ttu-id="a9337-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a9337-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9337-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9337-108">Attributes</span></span>

<span data-ttu-id="a9337-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a9337-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9337-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a9337-110">Child elements</span></span>

|<span data-ttu-id="a9337-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a9337-111">**Element**</span></span>|<span data-ttu-id="a9337-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9337-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9337-113">String</span><span class="sxs-lookup"><span data-stu-id="a9337-113">String</span></span>](string.md) <br/> |<span data-ttu-id="a9337-114">連絡先の子の名前を含みます。</span><span class="sxs-lookup"><span data-stu-id="a9337-114">Contains the name of a contact's child.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9337-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a9337-115">Parent elements</span></span>

|<span data-ttu-id="a9337-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9337-116">**Element**</span></span>|<span data-ttu-id="a9337-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9337-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9337-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="a9337-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a9337-119">Exchange ストア内の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="a9337-119">Represents a contact in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a9337-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a9337-120">Remarks</span></span>

<span data-ttu-id="a9337-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a9337-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9337-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a9337-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9337-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9337-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9337-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a9337-124">Schema name</span></span>  <br/> |<span data-ttu-id="a9337-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a9337-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9337-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a9337-126">Validation file</span></span>  <br/> |<span data-ttu-id="a9337-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a9337-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9337-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9337-128">Can be empty</span></span>  <br/> |<span data-ttu-id="a9337-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="a9337-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9337-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9337-130">See also</span></span>



- [<span data-ttu-id="a9337-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a9337-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


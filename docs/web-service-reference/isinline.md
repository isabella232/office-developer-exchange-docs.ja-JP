---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: IsInline 要素は、添付ファイルの項目内でのインラインで表示されているかどうかを表します。
ms.openlocfilehash: f2f9093777a3914de067ef63827de6cf354fc12d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832042"
---
# <a name="isinline"></a><span data-ttu-id="36ca7-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="36ca7-103">IsInline</span></span>

<span data-ttu-id="36ca7-104">**IsInline**要素は、添付ファイルの項目内でのインラインで表示されているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="36ca7-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="36ca7-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="36ca7-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36ca7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="36ca7-106">Attributes and elements</span></span>

<span data-ttu-id="36ca7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="36ca7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36ca7-108">属性</span><span class="sxs-lookup"><span data-stu-id="36ca7-108">Attributes</span></span>

<span data-ttu-id="36ca7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="36ca7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36ca7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="36ca7-110">Child elements</span></span>

<span data-ttu-id="36ca7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="36ca7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36ca7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="36ca7-112">Parent elements</span></span>

|<span data-ttu-id="36ca7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="36ca7-113">**Element**</span></span>|<span data-ttu-id="36ca7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="36ca7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36ca7-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="36ca7-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="36ca7-116">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="36ca7-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="36ca7-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="36ca7-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="36ca7-118">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="36ca7-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36ca7-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="36ca7-119">Text value</span></span>

<span data-ttu-id="36ca7-120">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="36ca7-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="36ca7-121">既定値は、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="36ca7-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36ca7-122">備考</span><span class="sxs-lookup"><span data-stu-id="36ca7-122">Remarks</span></span>

<span data-ttu-id="36ca7-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="36ca7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36ca7-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="36ca7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36ca7-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="36ca7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36ca7-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="36ca7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="36ca7-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="36ca7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="36ca7-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="36ca7-128">Validation File</span></span>  <br/> |<span data-ttu-id="36ca7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36ca7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36ca7-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="36ca7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="36ca7-131">False</span><span class="sxs-lookup"><span data-stu-id="36ca7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36ca7-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="36ca7-132">See also</span></span>



- [<span data-ttu-id="36ca7-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="36ca7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


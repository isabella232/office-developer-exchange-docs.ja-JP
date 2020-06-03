---
title: GroupType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c31552f-22b8-4bf0-8cac-046fd92ac0d4
description: GroupType 要素は、インスタントメッセージング (IM) グループのグループクラスを指定します。
ms.openlocfilehash: b8790a23507c51dfffceaddf3641ce820223c366
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462802"
---
# <a name="grouptype"></a><span data-ttu-id="8d1ca-103">GroupType</span><span class="sxs-lookup"><span data-stu-id="8d1ca-103">GroupType</span></span>

<span data-ttu-id="8d1ca-104">**GroupType**要素は、インスタントメッセージング (IM) グループのグループクラスを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-104">The **GroupType** element specifies the group class of an instant messaging (IM) group.</span></span> 
  
```XML
<GroupType></GroupType>
```

 <span data-ttu-id="8d1ca-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="8d1ca-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d1ca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8d1ca-106">Attributes and elements</span></span>

<span data-ttu-id="8d1ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d1ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d1ca-108">Attributes</span></span>

<span data-ttu-id="8d1ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d1ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d1ca-110">Child elements</span></span>

<span data-ttu-id="8d1ca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d1ca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d1ca-112">Parent elements</span></span>

|<span data-ttu-id="8d1ca-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d1ca-113">**Element**</span></span>|<span data-ttu-id="8d1ca-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d1ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d1ca-115">ImGroup</span><span class="sxs-lookup"><span data-stu-id="8d1ca-115">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="8d1ca-116">インスタントメッセージンググループを表します。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-116">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d1ca-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d1ca-117">Text value</span></span>

<span data-ttu-id="8d1ca-118">**GroupType**要素のテキスト値は、グループの種類を指定する文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-118">The text value of the **GroupType** element is a string value that specifies type of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8d1ca-119">注釈</span><span class="sxs-lookup"><span data-stu-id="8d1ca-119">Remarks</span></span>

<span data-ttu-id="8d1ca-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8d1ca-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d1ca-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8d1ca-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d1ca-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d1ca-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d1ca-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d1ca-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8d1ca-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="8d1ca-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="8d1ca-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d1ca-126">Validation File</span></span>  <br/> |<span data-ttu-id="8d1ca-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8d1ca-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d1ca-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8d1ca-128">Can Be Empty</span></span>  <br/> |<span data-ttu-id="8d1ca-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="8d1ca-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d1ca-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d1ca-130">See also</span></span>



- [<span data-ttu-id="8d1ca-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d1ca-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


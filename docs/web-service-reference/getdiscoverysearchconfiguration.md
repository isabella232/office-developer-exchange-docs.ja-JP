---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: GetDiscoverySearchConfiguration 要素は、電子的証拠開示検索の設定を取得する要求を指定します。
ms.openlocfilehash: 41a3cabb2822c4ee6a31aa7ff3074d62987edc92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760692"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="87799-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="87799-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="87799-104">**GetDiscoverySearchConfiguration**要素は、電子的証拠開示検索の設定を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="87799-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="87799-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="87799-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87799-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="87799-106">Attributes and elements</span></span>

<span data-ttu-id="87799-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="87799-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87799-108">属性</span><span class="sxs-lookup"><span data-stu-id="87799-108">Attributes</span></span>

<span data-ttu-id="87799-109">なし。</span><span class="sxs-lookup"><span data-stu-id="87799-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87799-110">子要素</span><span class="sxs-lookup"><span data-stu-id="87799-110">Child elements</span></span>

|<span data-ttu-id="87799-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="87799-111">**Element**</span></span>|<span data-ttu-id="87799-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="87799-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87799-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="87799-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="87799-114">検索の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="87799-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="87799-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="87799-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="87799-116">**GetSearchableMailboxes**要求から返されるグループのメンバーシップを展開するかどうかを示すブール値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="87799-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87799-117">親要素</span><span class="sxs-lookup"><span data-stu-id="87799-117">Parent elements</span></span>

<span data-ttu-id="87799-118">なし。</span><span class="sxs-lookup"><span data-stu-id="87799-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="87799-119">備考</span><span class="sxs-lookup"><span data-stu-id="87799-119">Remarks</span></span>

<span data-ttu-id="87799-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="87799-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="87799-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="87799-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87799-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="87799-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87799-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="87799-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87799-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="87799-124">Schema Name</span></span>  <br/> |<span data-ttu-id="87799-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="87799-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="87799-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="87799-126">Validation File</span></span>  <br/> |<span data-ttu-id="87799-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="87799-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87799-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="87799-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="87799-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="87799-129">See also</span></span>



- [<span data-ttu-id="87799-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="87799-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: GetDiscoverySearchConfiguration 要素は、電子情報開示検索の構成を取得する要求を指定します。
ms.openlocfilehash: 821c5e1429c160e326f6d99df3ff4fcc831b83d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461003"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="01ecf-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="01ecf-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="01ecf-104">**Getdiscoverysearchconfiguration**要素は、電子情報開示検索の構成を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="01ecf-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="01ecf-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="01ecf-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01ecf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01ecf-106">Attributes and elements</span></span>

<span data-ttu-id="01ecf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01ecf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01ecf-108">属性</span><span class="sxs-lookup"><span data-stu-id="01ecf-108">Attributes</span></span>

<span data-ttu-id="01ecf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="01ecf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01ecf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="01ecf-110">Child elements</span></span>

|<span data-ttu-id="01ecf-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="01ecf-111">**Element**</span></span>|<span data-ttu-id="01ecf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="01ecf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01ecf-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="01ecf-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="01ecf-114">検索の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="01ecf-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="01ecf-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="01ecf-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="01ecf-116">**Getsearchablemailemailrequest**要求から返されるグループのメンバーシップを拡張するかどうかを示すブール値を格納します。</span><span class="sxs-lookup"><span data-stu-id="01ecf-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01ecf-117">親要素</span><span class="sxs-lookup"><span data-stu-id="01ecf-117">Parent elements</span></span>

<span data-ttu-id="01ecf-118">なし。</span><span class="sxs-lookup"><span data-stu-id="01ecf-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01ecf-119">注釈</span><span class="sxs-lookup"><span data-stu-id="01ecf-119">Remarks</span></span>

<span data-ttu-id="01ecf-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="01ecf-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01ecf-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01ecf-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01ecf-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01ecf-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01ecf-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="01ecf-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01ecf-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01ecf-124">Schema Name</span></span>  <br/> |<span data-ttu-id="01ecf-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="01ecf-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="01ecf-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01ecf-126">Validation File</span></span>  <br/> |<span data-ttu-id="01ecf-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="01ecf-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01ecf-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01ecf-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="01ecf-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="01ecf-129">See also</span></span>



- [<span data-ttu-id="01ecf-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="01ecf-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


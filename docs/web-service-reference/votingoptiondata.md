---
title: VotingOptionData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 387328ae-4dcc-4230-8e4b-01d7894bbce2
description: VotingOptionData 要素は、各投票オプションに関する情報を指定します。
ms.openlocfilehash: f4240dc5c5d88e4964087b80e9081b93b41eed94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468650"
---
# <a name="votingoptiondata"></a><span data-ttu-id="37d44-103">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="37d44-103">VotingOptionData</span></span>

<span data-ttu-id="37d44-104">**VotingOptionData**要素は、各投票オプションに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="37d44-104">The **VotingOptionData** element specifies information about each voting option.</span></span> 
  
```XML
<VotingOptionData>
   <DisplayName/>
   <SendPrompt/>
</VotingOptionData>
```

 <span data-ttu-id="37d44-105">**VotingOptionDataType**</span><span class="sxs-lookup"><span data-stu-id="37d44-105">**VotingOptionDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37d44-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="37d44-106">Attributes and elements</span></span>

<span data-ttu-id="37d44-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="37d44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37d44-108">属性</span><span class="sxs-lookup"><span data-stu-id="37d44-108">Attributes</span></span>

<span data-ttu-id="37d44-109">なし。</span><span class="sxs-lookup"><span data-stu-id="37d44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37d44-110">子要素</span><span class="sxs-lookup"><span data-stu-id="37d44-110">Child elements</span></span>

<span data-ttu-id="37d44-111">[DisplayName (VotingOptionDataType)](displayname-votingoptiondatatype.md)  | [Sendprompt](sendprompt.md)</span><span class="sxs-lookup"><span data-stu-id="37d44-111">[DisplayName (VotingOptionDataType)](displayname-votingoptiondatatype.md) | [SendPrompt](sendprompt.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37d44-112">親要素</span><span class="sxs-lookup"><span data-stu-id="37d44-112">Parent elements</span></span>

[<span data-ttu-id="37d44-113">UserOptions</span><span class="sxs-lookup"><span data-stu-id="37d44-113">UserOptions</span></span>](useroptions.md)
  
## <a name="remarks"></a><span data-ttu-id="37d44-114">注釈</span><span class="sxs-lookup"><span data-stu-id="37d44-114">Remarks</span></span>

<span data-ttu-id="37d44-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="37d44-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="37d44-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="37d44-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37d44-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="37d44-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37d44-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="37d44-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37d44-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="37d44-119">Schema Name</span></span>  <br/> |<span data-ttu-id="37d44-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="37d44-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="37d44-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="37d44-121">Validation File</span></span>  <br/> |<span data-ttu-id="37d44-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="37d44-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37d44-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="37d44-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="37d44-124">正しい</span><span class="sxs-lookup"><span data-stu-id="37d44-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37d44-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="37d44-125">See also</span></span>



[<span data-ttu-id="37d44-126">UserOptions</span><span class="sxs-lookup"><span data-stu-id="37d44-126">UserOptions</span></span>](useroptions.md)


- [<span data-ttu-id="37d44-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="37d44-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


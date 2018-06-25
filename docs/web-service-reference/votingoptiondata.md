---
title: VotingOptionData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 387328ae-4dcc-4230-8e4b-01d7894bbce2
description: VotingOptionData 要素は、各投票のオプションについての情報を指定します。
ms.openlocfilehash: 743ddd7b2a7e8a0e86ab5973c71801b1ec19df19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839997"
---
# <a name="votingoptiondata"></a><span data-ttu-id="dd22f-103">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="dd22f-103">VotingOptionData</span></span>

<span data-ttu-id="dd22f-104">**VotingOptionData**要素は、各投票のオプションについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="dd22f-104">The **VotingOptionData** element specifies information about each voting option.</span></span> 
  
```XML
<VotingOptionData>
   <DisplayName/>
   <SendPrompt/>
</VotingOptionData>
```

 <span data-ttu-id="dd22f-105">**VotingOptionDataType**</span><span class="sxs-lookup"><span data-stu-id="dd22f-105">**VotingOptionDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd22f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd22f-106">Attributes and elements</span></span>

<span data-ttu-id="dd22f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd22f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd22f-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd22f-108">Attributes</span></span>

<span data-ttu-id="dd22f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd22f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd22f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd22f-110">Child elements</span></span>

<span data-ttu-id="dd22f-111">[表示名 (VotingOptionDataType)](displayname-votingoptiondatatype.md) | [SendPrompt](sendprompt.md)</span><span class="sxs-lookup"><span data-stu-id="dd22f-111">[DisplayName (VotingOptionDataType)](displayname-votingoptiondatatype.md) | [SendPrompt](sendprompt.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd22f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd22f-112">Parent elements</span></span>

[<span data-ttu-id="dd22f-113">UserOptions</span><span class="sxs-lookup"><span data-stu-id="dd22f-113">UserOptions</span></span>](useroptions.md)
  
## <a name="remarks"></a><span data-ttu-id="dd22f-114">備考</span><span class="sxs-lookup"><span data-stu-id="dd22f-114">Remarks</span></span>

<span data-ttu-id="dd22f-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dd22f-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="dd22f-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dd22f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd22f-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd22f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd22f-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd22f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd22f-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd22f-119">Schema Name</span></span>  <br/> |<span data-ttu-id="dd22f-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dd22f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd22f-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd22f-121">Validation File</span></span>  <br/> |<span data-ttu-id="dd22f-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd22f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd22f-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dd22f-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd22f-124">True</span><span class="sxs-lookup"><span data-stu-id="dd22f-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd22f-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd22f-125">See also</span></span>



[<span data-ttu-id="dd22f-126">UserOptions</span><span class="sxs-lookup"><span data-stu-id="dd22f-126">UserOptions</span></span>](useroptions.md)


- [<span data-ttu-id="dd22f-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd22f-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


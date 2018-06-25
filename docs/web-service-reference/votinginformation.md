---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: VotingInformation 要素は、返信のオプション、返信メッセージおよび承認要求メッセージの whereApproveandRejectare の投票の情報を指定します。
ms.openlocfilehash: f11c25bb1f3a3c4781cfa6c51e11ff87af40c7f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839990"
---
# <a name="votinginformation"></a><span data-ttu-id="6b68c-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="6b68c-103">VotingInformation</span></span>

<span data-ttu-id="6b68c-104">**VotingInformation**要素は、返信メッセージと、「承認」と「拒否」は、返信のオプションの承認要求のメッセージの返信の情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b68c-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="6b68c-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="6b68c-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b68c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b68c-106">Attributes and elements</span></span>

<span data-ttu-id="6b68c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b68c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b68c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b68c-108">Attributes</span></span>

<span data-ttu-id="6b68c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b68c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b68c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b68c-110">Child elements</span></span>

<span data-ttu-id="6b68c-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="6b68c-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b68c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6b68c-112">Parent elements</span></span>

[<span data-ttu-id="6b68c-113">Message</span><span class="sxs-lookup"><span data-stu-id="6b68c-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="6b68c-114">備考</span><span class="sxs-lookup"><span data-stu-id="6b68c-114">Remarks</span></span>

<span data-ttu-id="6b68c-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6b68c-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6b68c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b68c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b68c-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="6b68c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b68c-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="6b68c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b68c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b68c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="6b68c-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b68c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b68c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b68c-121">Validation File</span></span>  <br/> |<span data-ttu-id="6b68c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b68c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b68c-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6b68c-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b68c-124">True</span><span class="sxs-lookup"><span data-stu-id="6b68c-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b68c-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b68c-125">See also</span></span>



[<span data-ttu-id="6b68c-126">Message</span><span class="sxs-lookup"><span data-stu-id="6b68c-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="6b68c-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b68c-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


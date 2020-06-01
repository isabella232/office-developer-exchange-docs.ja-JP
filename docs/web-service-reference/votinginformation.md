---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: VotingInformation 要素は、投票メッセージと承認要求メッセージに関する投票情報を指定します。投票オプション whereApproveandRejectare ます。
ms.openlocfilehash: d946ba8c71d19c8cbb1befbe8c4e43e93590ccae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467747"
---
# <a name="votinginformation"></a><span data-ttu-id="246b7-103">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="246b7-103">VotingInformation</span></span>

<span data-ttu-id="246b7-104">**VotingInformation**要素は、投票メッセージと承認要求メッセージに関する投票情報を指定します。 "承認" および "却下" は投票オプションです。</span><span class="sxs-lookup"><span data-stu-id="246b7-104">The **VotingInformation** element specifies voting information on a voting message and approval request message where "Approve" and "Reject" are the voting options.</span></span> 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 <span data-ttu-id="246b7-105">**VotingInformationType**</span><span class="sxs-lookup"><span data-stu-id="246b7-105">**VotingInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="246b7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="246b7-106">Attributes and elements</span></span>

<span data-ttu-id="246b7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="246b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="246b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="246b7-108">Attributes</span></span>

<span data-ttu-id="246b7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="246b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="246b7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="246b7-110">Child elements</span></span>

<span data-ttu-id="246b7-111">[Useroptions](useroptions.md)  | [VotingResponse](votingresponse.md)</span><span class="sxs-lookup"><span data-stu-id="246b7-111">[UserOptions](useroptions.md) | [VotingResponse](votingresponse.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="246b7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="246b7-112">Parent elements</span></span>

[<span data-ttu-id="246b7-113">Message</span><span class="sxs-lookup"><span data-stu-id="246b7-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="246b7-114">注釈</span><span class="sxs-lookup"><span data-stu-id="246b7-114">Remarks</span></span>

<span data-ttu-id="246b7-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="246b7-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="246b7-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="246b7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="246b7-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="246b7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="246b7-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="246b7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="246b7-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="246b7-119">Schema Name</span></span>  <br/> |<span data-ttu-id="246b7-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="246b7-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="246b7-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="246b7-121">Validation File</span></span>  <br/> |<span data-ttu-id="246b7-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="246b7-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="246b7-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="246b7-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="246b7-124">正しい</span><span class="sxs-lookup"><span data-stu-id="246b7-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="246b7-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="246b7-125">See also</span></span>



[<span data-ttu-id="246b7-126">Message</span><span class="sxs-lookup"><span data-stu-id="246b7-126">Message</span></span>](message-ex15websvcsotherref.md)


- [<span data-ttu-id="246b7-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="246b7-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: UserOptions
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1acbb8a3-9110-4427-a06c-7e6e627e969f
description: UserOptions 要素は、メッセージに対する投票オプションの一覧を指定します。
ms.openlocfilehash: 2e0bbb373f423bbe9e913775b1f19d06dfd53f5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526761"
---
# <a name="useroptions"></a><span data-ttu-id="5ad1b-103">UserOptions</span><span class="sxs-lookup"><span data-stu-id="5ad1b-103">UserOptions</span></span>

<span data-ttu-id="5ad1b-104">**Useroptions**要素は、メッセージに対する投票オプションの一覧を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ad1b-104">The **UserOptions** element specifies the list of voting options on a message.</span></span> 
  
```XML
<UserOptions>
   <VotingOptionData>
</UserOptions>
```

 <span data-ttu-id="5ad1b-105">**ArrayOfVotingOptionDataType**</span><span class="sxs-lookup"><span data-stu-id="5ad1b-105">**ArrayOfVotingOptionDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ad1b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5ad1b-106">Attributes and elements</span></span>

<span data-ttu-id="5ad1b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ad1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ad1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ad1b-108">Attributes</span></span>

<span data-ttu-id="5ad1b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5ad1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ad1b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5ad1b-110">Child elements</span></span>

[<span data-ttu-id="5ad1b-111">VotingOptionData</span><span class="sxs-lookup"><span data-stu-id="5ad1b-111">VotingOptionData</span></span>](votingoptiondata.md)
  
### <a name="parent-elements"></a><span data-ttu-id="5ad1b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5ad1b-112">Parent elements</span></span>

[<span data-ttu-id="5ad1b-113">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="5ad1b-113">VotingInformation</span></span>](votinginformation.md)
  
## <a name="remarks"></a><span data-ttu-id="5ad1b-114">注釈</span><span class="sxs-lookup"><span data-stu-id="5ad1b-114">Remarks</span></span>

<span data-ttu-id="5ad1b-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5ad1b-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="5ad1b-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5ad1b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ad1b-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5ad1b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ad1b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ad1b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ad1b-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ad1b-119">Schema Name</span></span>  <br/> |<span data-ttu-id="5ad1b-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5ad1b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ad1b-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ad1b-121">Validation File</span></span>  <br/> |<span data-ttu-id="5ad1b-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5ad1b-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ad1b-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5ad1b-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ad1b-124">正しい</span><span class="sxs-lookup"><span data-stu-id="5ad1b-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ad1b-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ad1b-125">See also</span></span>



[<span data-ttu-id="5ad1b-126">VotingInformation</span><span class="sxs-lookup"><span data-stu-id="5ad1b-126">VotingInformation</span></span>](votinginformation.md)


- [<span data-ttu-id="5ad1b-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ad1b-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


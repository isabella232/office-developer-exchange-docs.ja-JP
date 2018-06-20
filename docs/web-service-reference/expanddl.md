---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: ExpandDL 要素は、配布リストを展開するための要求を定義します。
ms.openlocfilehash: ef93ed4684427a74a4fd2c38b4020ecb743fbaaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760369"
---
# <a name="expanddl"></a><span data-ttu-id="c2932-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="c2932-103">ExpandDL</span></span>

<span data-ttu-id="c2932-104">**ExpandDL**要素は、配布リストを展開するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="c2932-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="c2932-105">**ExpandDLType**</span><span class="sxs-lookup"><span data-stu-id="c2932-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2932-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c2932-106">Attributes and elements</span></span>

<span data-ttu-id="c2932-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2932-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2932-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2932-108">Attributes</span></span>

<span data-ttu-id="c2932-109">なし</span><span class="sxs-lookup"><span data-stu-id="c2932-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2932-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c2932-110">Child elements</span></span>

|<span data-ttu-id="c2932-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2932-111">**Element**</span></span>|<span data-ttu-id="c2932-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2932-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2932-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="c2932-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c2932-114">完全に解決された電子メール アドレスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="c2932-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="c2932-115">このメールボックスでは、展開する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c2932-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2932-116">親要素</span><span class="sxs-lookup"><span data-stu-id="c2932-116">Parent elements</span></span>

<span data-ttu-id="c2932-117">なし。</span><span class="sxs-lookup"><span data-stu-id="c2932-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2932-118">備考</span><span class="sxs-lookup"><span data-stu-id="c2932-118">Remarks</span></span>

<span data-ttu-id="c2932-119">1 つの配布リストの配布リストの展開のみ実行されます。</span><span class="sxs-lookup"><span data-stu-id="c2932-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="c2932-120">配布リストの展開は、再帰的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c2932-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="c2932-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c2932-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2932-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="c2932-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2932-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="c2932-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2932-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2932-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c2932-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c2932-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="c2932-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2932-126">Validation File</span></span>  <br/> |<span data-ttu-id="c2932-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2932-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2932-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2932-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2932-129">False</span><span class="sxs-lookup"><span data-stu-id="c2932-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2932-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2932-130">See also</span></span>



[<span data-ttu-id="c2932-131">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="c2932-131">ExpandDL operation</span></span>](expanddl-operation.md)


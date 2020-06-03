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
ms.openlocfilehash: 52b1ea1b51ce185c7a266e3002a4484e4b813bc0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456935"
---
# <a name="expanddl"></a><span data-ttu-id="8a7e2-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8a7e2-103">ExpandDL</span></span>

<span data-ttu-id="8a7e2-104">**Expanddl**要素は、配布リストを展開するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="8a7e2-105">**ExpandDLType**</span><span class="sxs-lookup"><span data-stu-id="8a7e2-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a7e2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8a7e2-106">Attributes and elements</span></span>

<span data-ttu-id="8a7e2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a7e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a7e2-108">Attributes</span></span>

<span data-ttu-id="8a7e2-109">なし</span><span class="sxs-lookup"><span data-stu-id="8a7e2-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a7e2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a7e2-110">Child elements</span></span>

|<span data-ttu-id="8a7e2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8a7e2-111">**Element**</span></span>|<span data-ttu-id="8a7e2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a7e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a7e2-113">メールボックス</span><span class="sxs-lookup"><span data-stu-id="8a7e2-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8a7e2-114">完全に解決された電子メールアドレスまたは配布リストを識別します。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="8a7e2-115">このメールボックスは、展開する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a7e2-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8a7e2-116">Parent elements</span></span>

<span data-ttu-id="8a7e2-117">なし。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a7e2-118">注釈</span><span class="sxs-lookup"><span data-stu-id="8a7e2-118">Remarks</span></span>

<span data-ttu-id="8a7e2-119">配布リストの展開は、1つの配布リストに対してのみ実行されます。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="8a7e2-120">配布リストの展開が再帰的ではありません。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="8a7e2-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8a7e2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a7e2-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8a7e2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a7e2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a7e2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a7e2-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a7e2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8a7e2-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8a7e2-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="8a7e2-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a7e2-126">Validation File</span></span>  <br/> |<span data-ttu-id="8a7e2-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8a7e2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a7e2-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8a7e2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a7e2-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="8a7e2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a7e2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="8a7e2-130">See also</span></span>



[<span data-ttu-id="8a7e2-131">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="8a7e2-131">ExpandDL operation</span></span>](expanddl-operation.md)


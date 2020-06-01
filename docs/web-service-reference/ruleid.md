---
title: RuleId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleId
api_type:
- schema
ms.assetid: 456e3c34-e536-456a-ac40-7fd4f94c0bad
description: RuleId 要素は、ルール識別子を指定します。
ms.openlocfilehash: 28fda7abbbbfd43be38d1ac4e5c37d37037993bc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464995"
---
# <a name="ruleid"></a><span data-ttu-id="56c04-103">RuleId</span><span class="sxs-lookup"><span data-stu-id="56c04-103">RuleId</span></span>

<span data-ttu-id="56c04-104">**RuleId**要素は、ルール識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="56c04-104">The **RuleId** element specifies a rule identifier.</span></span> 
  
```XML
<RuleId/>
```

 <span data-ttu-id="56c04-105">**string**</span><span class="sxs-lookup"><span data-stu-id="56c04-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56c04-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56c04-106">Attributes and elements</span></span>

<span data-ttu-id="56c04-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56c04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56c04-108">属性</span><span class="sxs-lookup"><span data-stu-id="56c04-108">Attributes</span></span>

<span data-ttu-id="56c04-109">なし。</span><span class="sxs-lookup"><span data-stu-id="56c04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56c04-110">子要素</span><span class="sxs-lookup"><span data-stu-id="56c04-110">Child elements</span></span>

<span data-ttu-id="56c04-111">なし。</span><span class="sxs-lookup"><span data-stu-id="56c04-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56c04-112">親要素</span><span class="sxs-lookup"><span data-stu-id="56c04-112">Parent elements</span></span>

|<span data-ttu-id="56c04-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="56c04-113">**Element**</span></span>|<span data-ttu-id="56c04-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="56c04-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56c04-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="56c04-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="56c04-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="56c04-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56c04-117">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="56c04-117">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="56c04-118">既存の受信トレイルールを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="56c04-118">Represents the operation to delete an existing Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56c04-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="56c04-119">Text value</span></span>

<span data-ttu-id="56c04-120">テキスト値は、ルールを表す文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="56c04-120">The text value is a string value that represents the rule.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56c04-121">注釈</span><span class="sxs-lookup"><span data-stu-id="56c04-121">Remarks</span></span>

<span data-ttu-id="56c04-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="56c04-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56c04-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="56c04-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56c04-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="56c04-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56c04-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56c04-125">Schema Name</span></span>  <br/> |<span data-ttu-id="56c04-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="56c04-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="56c04-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56c04-127">Validation File</span></span>  <br/> |<span data-ttu-id="56c04-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="56c04-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56c04-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="56c04-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="56c04-130">正しい</span><span class="sxs-lookup"><span data-stu-id="56c04-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56c04-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="56c04-131">See also</span></span>



- [<span data-ttu-id="56c04-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="56c04-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


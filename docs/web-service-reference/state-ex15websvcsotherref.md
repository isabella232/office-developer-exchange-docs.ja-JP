---
title: State
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- State
api_type:
- schema
ms.assetid: bcce7b0e-d504-4a1f-a530-db80b207f201
description: State 要素は、連絡先アイテムの居住状態を表します。
ms.openlocfilehash: 123aa0db83f58996924baadb0a87946db6934450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460002"
---
# <a name="state"></a><span data-ttu-id="581ca-103">State</span><span class="sxs-lookup"><span data-stu-id="581ca-103">State</span></span>

<span data-ttu-id="581ca-104">**State**要素は、連絡先アイテムの居住状態を表します。</span><span class="sxs-lookup"><span data-stu-id="581ca-104">The **State** element represents the state of residence for a contact item.</span></span> 
  
```xml
<State/>
```

<span data-ttu-id="581ca-105">**string**</span><span class="sxs-lookup"><span data-stu-id="581ca-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="581ca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="581ca-106">Attributes and elements</span></span>

<span data-ttu-id="581ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="581ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="581ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="581ca-108">Attributes</span></span>

<span data-ttu-id="581ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="581ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="581ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="581ca-110">Child elements</span></span>

<span data-ttu-id="581ca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="581ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="581ca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="581ca-112">Parent elements</span></span>

|<span data-ttu-id="581ca-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="581ca-113">**Element**</span></span>|<span data-ttu-id="581ca-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="581ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="581ca-115">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="581ca-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="581ca-116">連絡先アイテムの単一の物理アドレスを記述します。</span><span class="sxs-lookup"><span data-stu-id="581ca-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="581ca-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="581ca-117">Text value</span></span>

<span data-ttu-id="581ca-118">この要素を使用する場合は、状態の名前を表す文字列型 (string) の値が必要です。</span><span class="sxs-lookup"><span data-stu-id="581ca-118">A string value that represents the name of a state is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="581ca-119">注釈</span><span class="sxs-lookup"><span data-stu-id="581ca-119">Remarks</span></span>

<span data-ttu-id="581ca-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="581ca-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="581ca-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="581ca-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="581ca-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="581ca-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="581ca-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="581ca-123">Schema name</span></span>  <br/> |<span data-ttu-id="581ca-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="581ca-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="581ca-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="581ca-125">Validation file</span></span>  <br/> |<span data-ttu-id="581ca-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="581ca-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="581ca-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="581ca-127">Can be empty</span></span>  <br/> |<span data-ttu-id="581ca-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="581ca-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="581ca-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="581ca-129">See also</span></span>

- [<span data-ttu-id="581ca-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="581ca-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="581ca-131">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="581ca-131">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
- [<span data-ttu-id="581ca-132">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="581ca-132">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="581ca-133">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="581ca-133">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


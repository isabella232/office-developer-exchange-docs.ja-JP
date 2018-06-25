---
title: BusinessHomePage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BusinessHomePage
api_type:
- schema
ms.assetid: d7e16e32-c811-42d1-b6e9-cd9b7fbf3e0c
description: BusinessHomePage 要素は、連絡先のホーム ページ (Web アドレス) を表します。
ms.openlocfilehash: 2bd8fc791177116aed364dff9cd3e2e3c6dd0132
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759546"
---
# <a name="businesshomepage"></a><span data-ttu-id="5ffd0-103">BusinessHomePage</span><span class="sxs-lookup"><span data-stu-id="5ffd0-103">BusinessHomePage</span></span>

<span data-ttu-id="5ffd0-104">**BusinessHomePage**要素は、連絡先のホーム ページ (Web アドレス) を表します。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-104">The **BusinessHomePage** element represents the Home page (Web address) for the contact.</span></span> 
  
```xml
<BusinessHomePage/>
```

 <span data-ttu-id="5ffd0-105">**AnyUri**</span><span class="sxs-lookup"><span data-stu-id="5ffd0-105">**AnyUri**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ffd0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5ffd0-106">Attributes and elements</span></span>

<span data-ttu-id="5ffd0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ffd0-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ffd0-108">Attributes</span></span>

<span data-ttu-id="5ffd0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ffd0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5ffd0-110">Child elements</span></span>

<span data-ttu-id="5ffd0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5ffd0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5ffd0-112">Parent elements</span></span>

|<span data-ttu-id="5ffd0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ffd0-113">**Element**</span></span>|<span data-ttu-id="5ffd0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ffd0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ffd0-115">Contact</span><span class="sxs-lookup"><span data-stu-id="5ffd0-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5ffd0-116">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-116">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ffd0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5ffd0-117">Text value</span></span>

<span data-ttu-id="5ffd0-118">テキスト値は、ホーム ページの統一リソース識別子 (URI) を表します。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-118">The text value represents a uniform resource identifier (URI) for the Home page.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ffd0-119">備考</span><span class="sxs-lookup"><span data-stu-id="5ffd0-119">Remarks</span></span>

<span data-ttu-id="5ffd0-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ffd0-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="5ffd0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ffd0-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="5ffd0-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5ffd0-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ffd0-123">Schema name</span></span>  <br/> |<span data-ttu-id="5ffd0-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5ffd0-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="5ffd0-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ffd0-125">Validation file</span></span>  <br/> |<span data-ttu-id="5ffd0-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5ffd0-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5ffd0-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-127">Can be empty</span></span>  <br/> |<span data-ttu-id="5ffd0-128">False</span><span class="sxs-lookup"><span data-stu-id="5ffd0-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ffd0-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ffd0-129">See also</span></span>



- [<span data-ttu-id="5ffd0-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5ffd0-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5ffd0-131">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="5ffd0-131">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)


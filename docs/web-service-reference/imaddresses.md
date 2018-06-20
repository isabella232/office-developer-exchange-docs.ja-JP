---
title: ImAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: ImAddresses 要素は、連絡先のインスタント メッセージング アドレスのコレクションを表します。
ms.openlocfilehash: e8c7a22e8537a4526594042905f7bb8454238bf1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831861"
---
# <a name="imaddresses"></a><span data-ttu-id="b000d-103">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="b000d-103">ImAddresses</span></span>

<span data-ttu-id="b000d-104">**ImAddresses**要素は、連絡先のインスタント メッセージング アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="b000d-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="b000d-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="b000d-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b000d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b000d-106">Attributes and elements</span></span>

<span data-ttu-id="b000d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b000d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b000d-108">属性</span><span class="sxs-lookup"><span data-stu-id="b000d-108">Attributes</span></span>

<span data-ttu-id="b000d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b000d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b000d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b000d-110">Child elements</span></span>

|<span data-ttu-id="b000d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b000d-111">**Element**</span></span>|<span data-ttu-id="b000d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b000d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b000d-113">エントリ (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="b000d-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="b000d-114">インスタント メッセージングの連絡先のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="b000d-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b000d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b000d-115">Parent elements</span></span>

|<span data-ttu-id="b000d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b000d-116">**Element**</span></span>|<span data-ttu-id="b000d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b000d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b000d-118">Contact</span><span class="sxs-lookup"><span data-stu-id="b000d-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b000d-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b000d-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b000d-120">備考</span><span class="sxs-lookup"><span data-stu-id="b000d-120">Remarks</span></span>

<span data-ttu-id="b000d-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b000d-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b000d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="b000d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b000d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="b000d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b000d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b000d-124">Schema name</span></span>  <br/> |<span data-ttu-id="b000d-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b000d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b000d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b000d-126">Validation file</span></span>  <br/> |<span data-ttu-id="b000d-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b000d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b000d-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b000d-128">Can be empty</span></span>  <br/> |<span data-ttu-id="b000d-129">False</span><span class="sxs-lookup"><span data-stu-id="b000d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b000d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b000d-130">See also</span></span>



- [<span data-ttu-id="b000d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b000d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


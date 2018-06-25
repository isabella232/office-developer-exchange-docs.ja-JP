---
title: エントリ (IMAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: ee444170-7353-4e86-86c6-d7300a2f1777
description: エントリ要素は、インスタント メッセージング (IM) アドレスを連絡先を表します。
ms.openlocfilehash: 77de059cef470dde90ab0b929845cb260b4b867c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760325"
---
# <a name="entry-imaddress"></a><span data-ttu-id="8fb3b-103">エントリ (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="8fb3b-103">Entry (IMAddress)</span></span>

<span data-ttu-id="8fb3b-104">**エントリ**要素は、インスタント メッセージング (IM) アドレスを連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="8fb3b-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fb3b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8fb3b-106">Attributes and elements</span></span>

<span data-ttu-id="8fb3b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fb3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8fb3b-108">Attributes</span></span>

|<span data-ttu-id="8fb3b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-109">**Attribute**</span></span>|<span data-ttu-id="8fb3b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8fb3b-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-111">**Key**</span></span> <br/> | <span data-ttu-id="8fb3b-112">インスタント メッセージ アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="8fb3b-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="8fb3b-114">-ImAddress1</span><span class="sxs-lookup"><span data-stu-id="8fb3b-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="8fb3b-115">-ImAddress2</span><span class="sxs-lookup"><span data-stu-id="8fb3b-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="8fb3b-116">-ImAddress3</span><span class="sxs-lookup"><span data-stu-id="8fb3b-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8fb3b-117">子要素</span><span class="sxs-lookup"><span data-stu-id="8fb3b-117">Child elements</span></span>

<span data-ttu-id="8fb3b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fb3b-119">親要素</span><span class="sxs-lookup"><span data-stu-id="8fb3b-119">Parent elements</span></span>

|<span data-ttu-id="8fb3b-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-120">**Element**</span></span>|<span data-ttu-id="8fb3b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="8fb3b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fb3b-122">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="8fb3b-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="8fb3b-123">連絡先の IM アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fb3b-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8fb3b-124">Text value</span></span>

<span data-ttu-id="8fb3b-125">IM アドレスを表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fb3b-126">備考</span><span class="sxs-lookup"><span data-stu-id="8fb3b-126">Remarks</span></span>

<span data-ttu-id="8fb3b-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fb3b-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="8fb3b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fb3b-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="8fb3b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fb3b-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8fb3b-130">Schema name</span></span>  <br/> |<span data-ttu-id="8fb3b-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8fb3b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fb3b-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8fb3b-132">Validation file</span></span>  <br/> |<span data-ttu-id="8fb3b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fb3b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fb3b-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-134">Can be empty</span></span>  <br/> |<span data-ttu-id="8fb3b-135">False</span><span class="sxs-lookup"><span data-stu-id="8fb3b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fb3b-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="8fb3b-136">See also</span></span>

- [<span data-ttu-id="8fb3b-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8fb3b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="8fb3b-138">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-138">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="8fb3b-139">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="8fb3b-139">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="8fb3b-140">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fb3b-140">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


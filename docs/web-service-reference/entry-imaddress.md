---
title: Entry (IMAddress)
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
description: Entry 要素は、連絡先のインスタントメッセージング (IM) アドレスを表します。
ms.openlocfilehash: b6cc37447eb0f231e9e852a6c3cd64d6e1f3a89f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460702"
---
# <a name="entry-imaddress"></a><span data-ttu-id="b9b43-103">Entry (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="b9b43-103">Entry (IMAddress)</span></span>

<span data-ttu-id="b9b43-104">**Entry**要素は、連絡先のインスタントメッセージング (IM) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="b9b43-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="b9b43-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="b9b43-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9b43-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b9b43-106">Attributes and elements</span></span>

<span data-ttu-id="b9b43-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9b43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9b43-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9b43-108">Attributes</span></span>

|<span data-ttu-id="b9b43-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b9b43-109">**Attribute**</span></span>|<span data-ttu-id="b9b43-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9b43-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b9b43-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="b9b43-111">**Key**</span></span> <br/> | <span data-ttu-id="b9b43-112">IM アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="b9b43-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="b9b43-113">次に、この属性で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="b9b43-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="b9b43-114">- ImAddress1</span><span class="sxs-lookup"><span data-stu-id="b9b43-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="b9b43-115">- ImAddress2</span><span class="sxs-lookup"><span data-stu-id="b9b43-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="b9b43-116">- ImAddress3</span><span class="sxs-lookup"><span data-stu-id="b9b43-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b9b43-117">子要素</span><span class="sxs-lookup"><span data-stu-id="b9b43-117">Child elements</span></span>

<span data-ttu-id="b9b43-118">なし。</span><span class="sxs-lookup"><span data-stu-id="b9b43-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9b43-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b9b43-119">Parent elements</span></span>

|<span data-ttu-id="b9b43-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9b43-120">**Element**</span></span>|<span data-ttu-id="b9b43-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9b43-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9b43-122">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="b9b43-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="b9b43-123">連絡先の IM アドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="b9b43-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9b43-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9b43-124">Text value</span></span>

<span data-ttu-id="b9b43-125">この要素を使用する場合は、IM アドレスを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9b43-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9b43-126">注釈</span><span class="sxs-lookup"><span data-stu-id="b9b43-126">Remarks</span></span>

<span data-ttu-id="b9b43-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b9b43-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9b43-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b9b43-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9b43-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9b43-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9b43-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9b43-130">Schema name</span></span>  <br/> |<span data-ttu-id="b9b43-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9b43-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9b43-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9b43-132">Validation file</span></span>  <br/> |<span data-ttu-id="b9b43-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b9b43-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9b43-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9b43-134">Can be empty</span></span>  <br/> |<span data-ttu-id="b9b43-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="b9b43-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9b43-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9b43-136">See also</span></span>

- [<span data-ttu-id="b9b43-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b9b43-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b9b43-138">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="b9b43-138">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="b9b43-139">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="b9b43-139">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="b9b43-140">連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="b9b43-140">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)


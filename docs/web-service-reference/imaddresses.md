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
description: ImAddresses 要素は、連絡先のインスタントメッセージングアドレスのコレクションを表します。
ms.openlocfilehash: 24ff74d29c918d71116e25e097878b6e4e0a8ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460429"
---
# <a name="imaddresses"></a><span data-ttu-id="12b3f-103">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="12b3f-103">ImAddresses</span></span>

<span data-ttu-id="12b3f-104">**Imaddresses**要素は、連絡先のインスタントメッセージングアドレスのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="12b3f-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="12b3f-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="12b3f-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12b3f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="12b3f-106">Attributes and elements</span></span>

<span data-ttu-id="12b3f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12b3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12b3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="12b3f-108">Attributes</span></span>

<span data-ttu-id="12b3f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="12b3f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12b3f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="12b3f-110">Child elements</span></span>

|<span data-ttu-id="12b3f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="12b3f-111">**Element**</span></span>|<span data-ttu-id="12b3f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="12b3f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12b3f-113">Entry (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="12b3f-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="12b3f-114">連絡先のインスタントメッセージのアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="12b3f-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12b3f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="12b3f-115">Parent elements</span></span>

|<span data-ttu-id="12b3f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="12b3f-116">**Element**</span></span>|<span data-ttu-id="12b3f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="12b3f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12b3f-118">連絡先</span><span class="sxs-lookup"><span data-stu-id="12b3f-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="12b3f-119">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="12b3f-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12b3f-120">注釈</span><span class="sxs-lookup"><span data-stu-id="12b3f-120">Remarks</span></span>

<span data-ttu-id="12b3f-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="12b3f-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12b3f-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="12b3f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12b3f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="12b3f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12b3f-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12b3f-124">Schema name</span></span>  <br/> |<span data-ttu-id="12b3f-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="12b3f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="12b3f-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12b3f-126">Validation file</span></span>  <br/> |<span data-ttu-id="12b3f-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="12b3f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12b3f-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="12b3f-128">Can be empty</span></span>  <br/> |<span data-ttu-id="12b3f-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="12b3f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12b3f-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="12b3f-130">See also</span></span>



- [<span data-ttu-id="12b3f-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="12b3f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


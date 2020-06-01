---
title: UnknownEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntry
api_type:
- schema
ms.assetid: 3cb4c62e-052a-4326-8639-8c41dfd047b2
description: UnknownEntry 要素は、Active Directory ディレクトリサービスに対して解決できない単一の不明なアクセス許可エントリを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 452857690f719ba3ee9dffa29e576ca4f3b2b945
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459399"
---
# <a name="unknownentry"></a><span data-ttu-id="c5776-104">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="c5776-104">UnknownEntry</span></span>

<span data-ttu-id="c5776-105">**UnknownEntry**要素は、Active Directory ディレクトリサービスに対して解決できない単一の不明なアクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="c5776-105">The **UnknownEntry** element represents a single unknown permission entry that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="c5776-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c5776-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntry/>
```

 <span data-ttu-id="c5776-107">**string**</span><span class="sxs-lookup"><span data-stu-id="c5776-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5776-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5776-108">Attributes and elements</span></span>

<span data-ttu-id="c5776-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5776-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5776-110">属性</span><span class="sxs-lookup"><span data-stu-id="c5776-110">Attributes</span></span>

<span data-ttu-id="c5776-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c5776-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5776-112">子要素</span><span class="sxs-lookup"><span data-stu-id="c5776-112">Child elements</span></span>

<span data-ttu-id="c5776-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c5776-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5776-114">親要素</span><span class="sxs-lookup"><span data-stu-id="c5776-114">Parent elements</span></span>

|<span data-ttu-id="c5776-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5776-115">**Element**</span></span>|<span data-ttu-id="c5776-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5776-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5776-117">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="c5776-117">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="c5776-118">Active Directory に対して解決できない、不明なアクセス許可エントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5776-118">Contains an array of unknown permission entries that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="c5776-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c5776-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5776-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5776-120">Text value</span></span>

<span data-ttu-id="c5776-121">Text 値は、Active Directory に対して解決できないアクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="c5776-121">The text value represents a permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="c5776-122">テキスト値は、セキュリティ識別子 (SID) を表します。</span><span class="sxs-lookup"><span data-stu-id="c5776-122">The text value represents a security identifier (SID).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5776-123">注釈</span><span class="sxs-lookup"><span data-stu-id="c5776-123">Remarks</span></span>

<span data-ttu-id="c5776-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c5776-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5776-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5776-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5776-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5776-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5776-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5776-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c5776-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5776-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5776-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5776-129">Validation File</span></span>  <br/> |<span data-ttu-id="c5776-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5776-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5776-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c5776-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5776-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="c5776-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5776-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5776-133">See also</span></span>



- [<span data-ttu-id="c5776-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5776-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c5776-135">フォルダーレベルのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="c5776-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)


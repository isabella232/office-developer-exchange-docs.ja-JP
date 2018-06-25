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
description: UnknownEntry 要素は、Active Directory ディレクトリ サービスに対して解決することができない 1 つの不明なアクセス許可エントリを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 11939ad39c83ac2d15ec7fface6f530d3f60e12a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839810"
---
# <a name="unknownentry"></a><span data-ttu-id="16a18-104">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="16a18-104">UnknownEntry</span></span>

<span data-ttu-id="16a18-105">**UnknownEntry**要素は、Active Directory ディレクトリ サービスに対して解決することができない 1 つの不明なアクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="16a18-105">The **UnknownEntry** element represents a single unknown permission entry that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="16a18-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="16a18-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntry/>
```

 <span data-ttu-id="16a18-107">**string**</span><span class="sxs-lookup"><span data-stu-id="16a18-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16a18-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="16a18-108">Attributes and elements</span></span>

<span data-ttu-id="16a18-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16a18-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16a18-110">属性</span><span class="sxs-lookup"><span data-stu-id="16a18-110">Attributes</span></span>

<span data-ttu-id="16a18-111">なし。</span><span class="sxs-lookup"><span data-stu-id="16a18-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16a18-112">子要素</span><span class="sxs-lookup"><span data-stu-id="16a18-112">Child elements</span></span>

<span data-ttu-id="16a18-113">なし。</span><span class="sxs-lookup"><span data-stu-id="16a18-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16a18-114">親要素</span><span class="sxs-lookup"><span data-stu-id="16a18-114">Parent elements</span></span>

|<span data-ttu-id="16a18-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="16a18-115">**Element**</span></span>|<span data-ttu-id="16a18-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="16a18-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16a18-117">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="16a18-117">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="16a18-118">Active Directory に対して解決できない不明なアクセス許可エントリの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="16a18-118">Contains an array of unknown permission entries that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="16a18-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="16a18-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16a18-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="16a18-120">Text value</span></span>

<span data-ttu-id="16a18-121">テキスト値は、Active Directory に対して解決することはできませんが、アクセス許可エントリを表します。</span><span class="sxs-lookup"><span data-stu-id="16a18-121">The text value represents a permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="16a18-122">テキスト値は、セキュリティ識別子 (SID) を表します。</span><span class="sxs-lookup"><span data-stu-id="16a18-122">The text value represents a security identifier (SID).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="16a18-123">備考</span><span class="sxs-lookup"><span data-stu-id="16a18-123">Remarks</span></span>

<span data-ttu-id="16a18-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="16a18-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16a18-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="16a18-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16a18-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="16a18-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16a18-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16a18-127">Schema Name</span></span>  <br/> |<span data-ttu-id="16a18-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="16a18-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="16a18-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16a18-129">Validation File</span></span>  <br/> |<span data-ttu-id="16a18-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16a18-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16a18-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="16a18-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="16a18-132">False</span><span class="sxs-lookup"><span data-stu-id="16a18-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16a18-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="16a18-133">See also</span></span>



- [<span data-ttu-id="16a18-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="16a18-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="16a18-135">フォルダー レベルのアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="16a18-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)


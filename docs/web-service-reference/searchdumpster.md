---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: SearchDumpster 要素は、Exchange の収集機能で検索するかどうかを指定します。
ms.openlocfilehash: 4a40ee2da7fdaa4eaa3f5349545a0bfd3e13ba73
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833283"
---
# <a name="searchdumpster"></a><span data-ttu-id="9e1ad-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="9e1ad-103">SearchDumpster</span></span>

<span data-ttu-id="9e1ad-104">**SearchDumpster**要素は、Exchange の収集機能で検索するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="9e1ad-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9e1ad-105">Attributes and elements</span></span>

<span data-ttu-id="9e1ad-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e1ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e1ad-107">Attributes</span></span>

<span data-ttu-id="9e1ad-108">なし。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e1ad-109">子要素</span><span class="sxs-lookup"><span data-stu-id="9e1ad-109">Child elements</span></span>

<span data-ttu-id="9e1ad-110">なし。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e1ad-111">親要素</span><span class="sxs-lookup"><span data-stu-id="9e1ad-111">Parent elements</span></span>

[<span data-ttu-id="9e1ad-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="9e1ad-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="9e1ad-113">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e1ad-113">Text value</span></span>

<span data-ttu-id="9e1ad-114">の**場合は true** 、 **SearchDumpster**要素のテキスト値は、メールボックスの統計情報の検索に Exchange の収集機能が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="9e1ad-115">**False**の値は、Exchange の収集機能が検索されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9e1ad-116">備考</span><span class="sxs-lookup"><span data-stu-id="9e1ad-116">Remarks</span></span>

<span data-ttu-id="9e1ad-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e1ad-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e1ad-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="9e1ad-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e1ad-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="9e1ad-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e1ad-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e1ad-121">Schema name</span></span>  <br/> |<span data-ttu-id="9e1ad-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9e1ad-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e1ad-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e1ad-123">Validation file</span></span>  <br/> |<span data-ttu-id="9e1ad-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e1ad-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e1ad-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9e1ad-125">Can be empty</span></span>  <br/> ||
   


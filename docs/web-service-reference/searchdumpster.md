---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: SearchDumpster 要素は、Exchange の収集で検索するかどうかを指定します。
ms.openlocfilehash: 067bf8ea3e589aa392c6b8ba6d4dc10b430c1f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460492"
---
# <a name="searchdumpster"></a><span data-ttu-id="2b3be-103">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="2b3be-103">SearchDumpster</span></span>

<span data-ttu-id="2b3be-104">**Searchdumpster**要素は、Exchange の収集で検索するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b3be-104">The **SearchDumpster** element specifies whether to search in the Exchange Dumpster.</span></span> 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="2b3be-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2b3be-105">Attributes and elements</span></span>

<span data-ttu-id="2b3be-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b3be-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b3be-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b3be-107">Attributes</span></span>

<span data-ttu-id="2b3be-108">なし。</span><span class="sxs-lookup"><span data-stu-id="2b3be-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b3be-109">子要素</span><span class="sxs-lookup"><span data-stu-id="2b3be-109">Child elements</span></span>

<span data-ttu-id="2b3be-110">なし。</span><span class="sxs-lookup"><span data-stu-id="2b3be-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b3be-111">親要素</span><span class="sxs-lookup"><span data-stu-id="2b3be-111">Parent elements</span></span>

[<span data-ttu-id="2b3be-112">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="2b3be-112">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a><span data-ttu-id="2b3be-113">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2b3be-113">Text value</span></span>

<span data-ttu-id="2b3be-114">**Searchdumpster**要素のテキスト値が**true**の場合は、メールボックス統計検索に Exchange の収集が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="2b3be-114">A text value of **true** for the **SearchDumpster** element indicates that the mailbox statistics search includes the Exchange Dumpster.</span></span> <span data-ttu-id="2b3be-115">値が**false**の場合は、Exchange の収集が検索されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2b3be-115">A value of **false** indicates that the Exchange Dumpster is not searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2b3be-116">注釈</span><span class="sxs-lookup"><span data-stu-id="2b3be-116">Remarks</span></span>

<span data-ttu-id="2b3be-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2b3be-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b3be-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2b3be-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b3be-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2b3be-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b3be-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b3be-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b3be-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b3be-121">Schema name</span></span>  <br/> |<span data-ttu-id="2b3be-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2b3be-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b3be-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b3be-123">Validation file</span></span>  <br/> |<span data-ttu-id="2b3be-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2b3be-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b3be-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b3be-125">Can be empty</span></span>  <br/> ||
   


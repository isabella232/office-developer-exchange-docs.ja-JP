---
title: 追加アイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: この要素には、インデックスを作成できないアイテムを含めるかどうかを示すブール値が含まれています。
ms.openlocfilehash: eab559e938f0b949d79626ae5bf61b3d4a838924
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460625"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="cd7ab-103">追加アイテム</span><span class="sxs-lookup"><span data-stu-id="cd7ab-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="cd7ab-104">この**要素には、** インデックスを作成できないアイテムを含めるかどうかを示す**ブール**値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="cd7ab-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cd7ab-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd7ab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cd7ab-106">Attributes and elements</span></span>

<span data-ttu-id="cd7ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd7ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd7ab-108">Attributes</span></span>

<span data-ttu-id="cd7ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd7ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cd7ab-110">Child elements</span></span>

<span data-ttu-id="cd7ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd7ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cd7ab-112">Parent elements</span></span>

[<span data-ttu-id="cd7ab-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="cd7ab-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="cd7ab-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cd7ab-114">Text value</span></span>

<span data-ttu-id="cd7ab-115">リスト**アイテム**の文字列値が**true**の場合は、インデックスを作成できないアイテムがメールボックス保持に含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="cd7ab-116">値が**false**の場合、インデックス付けできないアイテムはメールボックス保持に含まれないことを示します。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cd7ab-117">注釈</span><span class="sxs-lookup"><span data-stu-id="cd7ab-117">Remarks</span></span>

<span data-ttu-id="cd7ab-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cd7ab-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd7ab-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cd7ab-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd7ab-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd7ab-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cd7ab-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cd7ab-122">Schema name</span></span>  <br/> |<span data-ttu-id="cd7ab-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cd7ab-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cd7ab-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cd7ab-124">Validation file</span></span>  <br/> |<span data-ttu-id="cd7ab-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cd7ab-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cd7ab-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd7ab-126">Can be empty</span></span>  <br/> |<span data-ttu-id="cd7ab-127">false</span><span class="sxs-lookup"><span data-stu-id="cd7ab-127">false</span></span>  <br/> |
   


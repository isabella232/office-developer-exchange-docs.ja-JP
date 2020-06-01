---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: MakeItemImmutable 要素は、アイテムを読み取り専用にする必要があるかどうかを示すブール値を指定します。
ms.openlocfilehash: 05c6e3343b8ba892048174ad98c9d31fe8da685b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465864"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="9d369-103">MakeItemImmutable</span><span class="sxs-lookup"><span data-stu-id="9d369-103">MakeItemImmutable</span></span>

<span data-ttu-id="9d369-104">**Makeitemimmutable**要素は、アイテムを読み取り専用にする必要があるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d369-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="9d369-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9d369-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d369-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9d369-106">Attributes and elements</span></span>

<span data-ttu-id="9d369-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d369-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d369-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d369-108">Attributes</span></span>

<span data-ttu-id="9d369-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d369-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d369-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d369-110">Child elements</span></span>

<span data-ttu-id="9d369-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9d369-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d369-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d369-112">Parent elements</span></span>

[<span data-ttu-id="9d369-113">Updateitemin回復可能アイテム</span><span class="sxs-lookup"><span data-stu-id="9d369-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="9d369-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d369-114">Text value</span></span>

<span data-ttu-id="9d369-115">**Makeitemimmutable**要素のテキスト値が**true**になっている場合は、アイテムを読み取り専用にする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9d369-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="9d369-116">値が**false**の場合は、アイテムに読み取り/書き込みアクセスが許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9d369-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d369-117">注釈</span><span class="sxs-lookup"><span data-stu-id="9d369-117">Remarks</span></span>

<span data-ttu-id="9d369-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d369-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d369-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d369-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d369-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9d369-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d369-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d369-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d369-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d369-122">Schema name</span></span>  <br/> |<span data-ttu-id="9d369-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d369-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d369-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d369-124">Validation file</span></span>  <br/> |<span data-ttu-id="9d369-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9d369-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d369-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9d369-126">Can be empty</span></span>  <br/> ||
   


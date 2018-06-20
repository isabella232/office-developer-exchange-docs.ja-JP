---
title: プレビュー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d33f557-c9d5-4f7f-82c0-d800412f8b7e
description: '[プレビューの表示項目の最初の 256 文字を指定します。'
ms.openlocfilehash: 38589f8d8efb58e109de59ebf9b5e56556ab58af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832876"
---
# <a name="preview"></a><span data-ttu-id="5a2ce-103">プレビュー</span><span class="sxs-lookup"><span data-stu-id="5a2ce-103">Preview</span></span>

<span data-ttu-id="5a2ce-104">**[プレビュー**の表示項目の最初の 256 文字を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-104">The **Preview** element specifies the first 256 characters of an item for display.</span></span> 
  
```XML
<Preview></Preview>
```

 <span data-ttu-id="5a2ce-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5a2ce-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a2ce-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5a2ce-106">Attributes and elements</span></span>

<span data-ttu-id="5a2ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a2ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a2ce-108">Attributes</span></span>

<span data-ttu-id="5a2ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a2ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a2ce-110">Child elements</span></span>

<span data-ttu-id="5a2ce-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a2ce-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a2ce-112">Parent elements</span></span>

<span data-ttu-id="5a2ce-113">[会話 (ConversationType)](conversation-conversationtype.md) | [SearchPreviewItem](searchpreviewitem.md) | [アイテム](item.md) | [連絡先](contact.md) | [メッセージ](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="5a2ce-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5a2ce-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a2ce-114">Text value</span></span>

<span data-ttu-id="5a2ce-115">プレビュー要素のテキスト値は、項目の最初の 256 文字です。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-115">The text value of the Preview element is the first 256 characters of the item.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a2ce-116">備考</span><span class="sxs-lookup"><span data-stu-id="5a2ce-116">Remarks</span></span>

<span data-ttu-id="5a2ce-117">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5a2ce-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a2ce-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="5a2ce-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a2ce-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="5a2ce-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a2ce-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a2ce-121">Schema name</span></span>  <br/> |<span data-ttu-id="5a2ce-122">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5a2ce-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a2ce-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a2ce-123">Validation file</span></span>  <br/> |<span data-ttu-id="5a2ce-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5a2ce-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a2ce-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5a2ce-125">Can be empty</span></span>  <br/> ||
   


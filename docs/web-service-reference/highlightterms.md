---
title: HighlightTerms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce4a2978-fd0c-41a4-ae65-aa6f5dc9a0f9
description: HighlightTerms 要素は、強調表示された FindItem 操作および FindConversation 操作の応答で返される条件を識別します。
ms.openlocfilehash: c075e63674bc08773925a2a540a1c2434423926d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831808"
---
# <a name="highlightterms"></a><span data-ttu-id="fcff3-103">HighlightTerms</span><span class="sxs-lookup"><span data-stu-id="fcff3-103">HighlightTerms</span></span>

<span data-ttu-id="fcff3-104">**HighlightTerms**要素は、強調表示された**FindItem**操作および**FindConversation**操作の応答で返される条件を識別します。</span><span class="sxs-lookup"><span data-stu-id="fcff3-104">The **HighlightTerms** element identifies the highlighted terms returned in a **FindItem** operation and a **FindConversation** operation response.</span></span> 
  
```XML
<HighlightTerms>
   <Term/>
</HighlightTerms>
```

 <span data-ttu-id="fcff3-105">**ArrayOfHighlightTermsType**</span><span class="sxs-lookup"><span data-stu-id="fcff3-105">**ArrayOfHighlightTermsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcff3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fcff3-106">Attributes and elements</span></span>

<span data-ttu-id="fcff3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fcff3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcff3-108">属性</span><span class="sxs-lookup"><span data-stu-id="fcff3-108">Attributes</span></span>

<span data-ttu-id="fcff3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fcff3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcff3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fcff3-110">Child elements</span></span>

<span data-ttu-id="fcff3-111">用語</span><span class="sxs-lookup"><span data-stu-id="fcff3-111">Term</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fcff3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fcff3-112">Parent elements</span></span>

<span data-ttu-id="fcff3-113">[FindConversationResponse](findconversationresponse.md) | [FindItemResponseMessage](finditemresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="fcff3-113">[FindConversationResponse](findconversationresponse.md) | [FindItemResponseMessage](finditemresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fcff3-114">備考</span><span class="sxs-lookup"><span data-stu-id="fcff3-114">Remarks</span></span>

<span data-ttu-id="fcff3-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fcff3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fcff3-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fcff3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcff3-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="fcff3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcff3-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="fcff3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fcff3-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fcff3-119">Schema name</span></span>  <br/> |<span data-ttu-id="fcff3-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fcff3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fcff3-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fcff3-121">Validation file</span></span>  <br/> |<span data-ttu-id="fcff3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fcff3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fcff3-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fcff3-123">Can be empty</span></span>  <br/> ||
   


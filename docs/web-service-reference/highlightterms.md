---
title: HighlightTerms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce4a2978-fd0c-41a4-ae65-aa6f5dc9a0f9
description: HighlightTerms 要素は、FindItem 操作で返される強調表示された用語および FindConversation 操作の応答を識別します。
ms.openlocfilehash: c55ffc010dc0cfb09403433aaf8a0809a26f71a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457635"
---
# <a name="highlightterms"></a><span data-ttu-id="2a13a-103">HighlightTerms</span><span class="sxs-lookup"><span data-stu-id="2a13a-103">HighlightTerms</span></span>

<span data-ttu-id="2a13a-104">**HighlightTerms**要素は、 **FindItem**操作で返される強調表示された用語および**findconversation**操作の応答を識別します。</span><span class="sxs-lookup"><span data-stu-id="2a13a-104">The **HighlightTerms** element identifies the highlighted terms returned in a **FindItem** operation and a **FindConversation** operation response.</span></span> 
  
```XML
<HighlightTerms>
   <Term/>
</HighlightTerms>
```

 <span data-ttu-id="2a13a-105">**ArrayOfHighlightTermsType**</span><span class="sxs-lookup"><span data-stu-id="2a13a-105">**ArrayOfHighlightTermsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a13a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a13a-106">Attributes and elements</span></span>

<span data-ttu-id="2a13a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a13a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a13a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a13a-108">Attributes</span></span>

<span data-ttu-id="2a13a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2a13a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a13a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2a13a-110">Child elements</span></span>

<span data-ttu-id="2a13a-111">用語</span><span class="sxs-lookup"><span data-stu-id="2a13a-111">Term</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a13a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2a13a-112">Parent elements</span></span>

<span data-ttu-id="2a13a-113">[FindConversationResponse](findconversationresponse.md)  | [FindItemResponseMessage](finditemresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="2a13a-113">[FindConversationResponse](findconversationresponse.md) | [FindItemResponseMessage](finditemresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2a13a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="2a13a-114">Remarks</span></span>

<span data-ttu-id="2a13a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2a13a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a13a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a13a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a13a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2a13a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a13a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a13a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2a13a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a13a-119">Schema name</span></span>  <br/> |<span data-ttu-id="2a13a-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2a13a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2a13a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a13a-121">Validation file</span></span>  <br/> |<span data-ttu-id="2a13a-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2a13a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a13a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a13a-123">Can be empty</span></span>  <br/> ||
   


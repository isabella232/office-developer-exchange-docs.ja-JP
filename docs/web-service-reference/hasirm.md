---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 要素は、会話内の少なくとも1つのメッセージと現在のフォルダーが IRM で保護されたメッセージであるかどうかを指定します。
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462781"
---
# <a name="hasirm"></a><span data-ttu-id="e9440-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="e9440-103">HasIrm</span></span>

<span data-ttu-id="e9440-104">**Hasirm**要素は、会話内の少なくとも1つのメッセージと現在のフォルダーが IRM で保護されたメッセージであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9440-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="e9440-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e9440-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9440-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9440-106">Attributes and elements</span></span>

<span data-ttu-id="e9440-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9440-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9440-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9440-108">Attributes</span></span>

<span data-ttu-id="e9440-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9440-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9440-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9440-110">Child elements</span></span>

<span data-ttu-id="e9440-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e9440-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e9440-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e9440-112">Parent elements</span></span>

[<span data-ttu-id="e9440-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e9440-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="e9440-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e9440-114">Text value</span></span>

<span data-ttu-id="e9440-115">スレッドに少なくとも1つのメッセージがあり、現在のフォルダーに IRM がある場合は、 **Hasirm**要素のテキスト値は**true**です。</span><span class="sxs-lookup"><span data-stu-id="e9440-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="e9440-116">それ以外の場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="e9440-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e9440-117">注釈</span><span class="sxs-lookup"><span data-stu-id="e9440-117">Remarks</span></span>

<span data-ttu-id="e9440-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e9440-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e9440-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e9440-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9440-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9440-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9440-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9440-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9440-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9440-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e9440-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9440-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9440-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9440-124">Validation File</span></span>  <br/> |<span data-ttu-id="e9440-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9440-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9440-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9440-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9440-127">正しい</span><span class="sxs-lookup"><span data-stu-id="e9440-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9440-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9440-128">See also</span></span>



[<span data-ttu-id="e9440-129">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e9440-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="e9440-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e9440-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: RetentionPolicyType 要素は、会話内のアイテムに適用される保持ポリシーの種類を指定します。
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833229"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="92d93-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="92d93-103">RetentionPolicyType</span></span>

<span data-ttu-id="92d93-104">**RetentionPolicyType**要素は、会話内のアイテムに適用される保持ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="92d93-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="92d93-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="92d93-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92d93-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="92d93-106">Attributes and elements</span></span>

<span data-ttu-id="92d93-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92d93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92d93-108">属性</span><span class="sxs-lookup"><span data-stu-id="92d93-108">Attributes</span></span>

<span data-ttu-id="92d93-109">なし。</span><span class="sxs-lookup"><span data-stu-id="92d93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92d93-110">子要素</span><span class="sxs-lookup"><span data-stu-id="92d93-110">Child elements</span></span>

<span data-ttu-id="92d93-111">なし。</span><span class="sxs-lookup"><span data-stu-id="92d93-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92d93-112">親要素</span><span class="sxs-lookup"><span data-stu-id="92d93-112">Parent elements</span></span>

[<span data-ttu-id="92d93-113">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="92d93-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="92d93-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="92d93-114">Text value</span></span>

<span data-ttu-id="92d93-115">**RetentionPolicyType**要素のテキスト値は、会話内のアイテムに適用される保持型です。</span><span class="sxs-lookup"><span data-stu-id="92d93-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="92d93-116">**削除**のテキスト値は、保持期限が切れると、会話内の項目が削除されることを示します。</span><span class="sxs-lookup"><span data-stu-id="92d93-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="92d93-117">**アーカイブ**のテキスト値は、保持期限が切れると、会話内の項目をアーカイブ メールボックスに移動したことを示します。</span><span class="sxs-lookup"><span data-stu-id="92d93-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="92d93-118">備考</span><span class="sxs-lookup"><span data-stu-id="92d93-118">Remarks</span></span>

<span data-ttu-id="92d93-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92d93-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="92d93-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="92d93-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92d93-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="92d93-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92d93-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="92d93-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92d93-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92d93-123">Schema name</span></span>  <br/> |<span data-ttu-id="92d93-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="92d93-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="92d93-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92d93-125">Validation file</span></span>  <br/> |<span data-ttu-id="92d93-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92d93-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92d93-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="92d93-127">Can be empty</span></span>  <br/> ||
   


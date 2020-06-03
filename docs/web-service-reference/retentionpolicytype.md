---
title: RetentionPolicyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: RetentionPolicyType 要素は、スレッド内のアイテムに適用されるアイテム保持ポリシーの種類を指定します。
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462872"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="fa5f2-103">RetentionPolicyType</span><span class="sxs-lookup"><span data-stu-id="fa5f2-103">RetentionPolicyType</span></span>

<span data-ttu-id="fa5f2-104">**RetentionPolicyType**要素は、スレッド内のアイテムに適用されるアイテム保持ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="fa5f2-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="fa5f2-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa5f2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fa5f2-106">Attributes and elements</span></span>

<span data-ttu-id="fa5f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa5f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa5f2-108">Attributes</span></span>

<span data-ttu-id="fa5f2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa5f2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fa5f2-110">Child elements</span></span>

<span data-ttu-id="fa5f2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa5f2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fa5f2-112">Parent elements</span></span>

[<span data-ttu-id="fa5f2-113">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="fa5f2-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="fa5f2-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fa5f2-114">Text value</span></span>

<span data-ttu-id="fa5f2-115">**RetentionPolicyType**要素のテキスト値は、会話内のアイテムに適用される保持タイプです。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="fa5f2-116">[**削除**] のテキスト値は、保持保持期間の期限が切れたときにスレッド内のアイテムが削除されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="fa5f2-117">**Archive**のテキスト値は、保持保持期間が経過すると、スレッド内のアイテムがアーカイブメールボックスに移動されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fa5f2-118">注釈</span><span class="sxs-lookup"><span data-stu-id="fa5f2-118">Remarks</span></span>

<span data-ttu-id="fa5f2-119">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa5f2-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa5f2-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fa5f2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa5f2-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa5f2-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa5f2-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa5f2-123">Schema name</span></span>  <br/> |<span data-ttu-id="fa5f2-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fa5f2-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa5f2-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa5f2-125">Validation file</span></span>  <br/> |<span data-ttu-id="fa5f2-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fa5f2-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa5f2-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa5f2-127">Can be empty</span></span>  <br/> ||
   


---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Type 要素は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465108"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="339a6-103">Type (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="339a6-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="339a6-104">**Type**要素は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="339a6-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="339a6-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="339a6-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="339a6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="339a6-106">Attributes and elements</span></span>

<span data-ttu-id="339a6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="339a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="339a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="339a6-108">Attributes</span></span>

<span data-ttu-id="339a6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="339a6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="339a6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="339a6-110">Child elements</span></span>

<span data-ttu-id="339a6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="339a6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="339a6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="339a6-112">Parent elements</span></span>

[<span data-ttu-id="339a6-113">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="339a6-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="339a6-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="339a6-114">Text value</span></span>

<span data-ttu-id="339a6-115">**Type**要素のテキスト値は、アイテム保持ポリシーで使用されるフォルダーの種類です。</span><span class="sxs-lookup"><span data-stu-id="339a6-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="339a6-116">テキスト値には、既定のフォルダーの種類を表す次のいずれかの値を指定できます: Calendar、Contacts、DeletedItems、下書き、受信トレイ、JunkEmail、Journal、Notes、送信トレイ、SentItems、Tasks、All、ManagedCustomFolder、RssSubscriptions、SyncIssues、ConversationHistory、Personal、Ableitems、または NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="339a6-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="339a6-117">注釈</span><span class="sxs-lookup"><span data-stu-id="339a6-117">Remarks</span></span>

<span data-ttu-id="339a6-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="339a6-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="339a6-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="339a6-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="339a6-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="339a6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="339a6-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="339a6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="339a6-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="339a6-122">Schema name</span></span>  <br/> |<span data-ttu-id="339a6-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="339a6-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="339a6-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="339a6-124">Validation file</span></span>  <br/> |<span data-ttu-id="339a6-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="339a6-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="339a6-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="339a6-126">Can be empty</span></span>  <br/> |<span data-ttu-id="339a6-127">false</span><span class="sxs-lookup"><span data-stu-id="339a6-127">false</span></span>  <br/> |
   


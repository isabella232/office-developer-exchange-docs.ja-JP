---
title: 型 (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: 型の要素では、リテンション ・ ポリシーで使用されているフォルダーの種類を指定します。
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839756"
---
# <a name="type-elcfoldertype"></a><span data-ttu-id="ce3bc-103">型 (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="ce3bc-103">Type (ElcFolderType)</span></span>

<span data-ttu-id="ce3bc-104">**型**の要素では、リテンション ・ ポリシーで使用されているフォルダーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-104">The **Type** element specifies the type of folder used in a retention policy.</span></span> 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 <span data-ttu-id="ce3bc-105">**ElcFolderType**</span><span class="sxs-lookup"><span data-stu-id="ce3bc-105">**ElcFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce3bc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ce3bc-106">Attributes and elements</span></span>

<span data-ttu-id="ce3bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce3bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce3bc-108">Attributes</span></span>

<span data-ttu-id="ce3bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce3bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ce3bc-110">Child elements</span></span>

<span data-ttu-id="ce3bc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce3bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ce3bc-112">Parent elements</span></span>

[<span data-ttu-id="ce3bc-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="ce3bc-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="ce3bc-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ce3bc-114">Text value</span></span>

<span data-ttu-id="ce3bc-115">**型**の要素のテキスト値は、リテンション ・ ポリシーで使用されているフォルダーの種類です。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-115">The text value of the **Type** element is the folder type used in a retention policy.</span></span> <span data-ttu-id="ce3bc-116">テキスト値には、既定のフォルダーの種類を表す次の値のいずれかを指定できます: 予定表、連絡先、DeletedItems、下書き、受信トレイ、JunkEmail、ジャーナル、メモ、送信トレイ、送信済みアイテム、タスク、すべて、ManagedCustomFolder、RssSubscriptions、SyncIssues、ConversationHistory、個人、RecoverableItems、または NonIpmRoot</span><span class="sxs-lookup"><span data-stu-id="ce3bc-116">The text value can be one of the following values that represent a default folder type: Calendar, Contacts, DeletedItems, Drafts, Inbox, JunkEmail, Journal, Notes, Outbox, SentItems, Tasks, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, Personal, RecoverableItems, or NonIpmRoot</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ce3bc-117">備考</span><span class="sxs-lookup"><span data-stu-id="ce3bc-117">Remarks</span></span>

<span data-ttu-id="ce3bc-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ce3bc-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce3bc-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="ce3bc-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce3bc-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="ce3bc-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce3bc-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce3bc-122">Schema name</span></span>  <br/> |<span data-ttu-id="ce3bc-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ce3bc-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce3bc-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce3bc-124">Validation file</span></span>  <br/> |<span data-ttu-id="ce3bc-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce3bc-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce3bc-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ce3bc-126">Can be empty</span></span>  <br/> |<span data-ttu-id="ce3bc-127">false</span><span class="sxs-lookup"><span data-stu-id="ce3bc-127">false</span></span>  <br/> |
   


---
title: ファイアウォール (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: ファイアウォールの要素では、保留リストの動作の種類を示します。
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759268"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="0d5ff-103">ファイアウォール (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="0d5ff-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="0d5ff-104">**ファイアウォール**の要素では、保留リストの動作の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="0d5ff-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="0d5ff-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d5ff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0d5ff-106">Attributes and elements</span></span>

<span data-ttu-id="0d5ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d5ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d5ff-108">Attributes</span></span>

<span data-ttu-id="0d5ff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d5ff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0d5ff-110">Child elements</span></span>

<span data-ttu-id="0d5ff-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d5ff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0d5ff-112">Parent elements</span></span>

[<span data-ttu-id="0d5ff-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0d5ff-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="0d5ff-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0d5ff-114">Text value</span></span>

<span data-ttu-id="0d5ff-115">**ファイアウォール**の要素のテキスト値は、保留中のメールボックスの設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="0d5ff-116">**作成する**テキスト値は、メールボックスの保留リストを作成することを示します。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="0d5ff-117">**更新プログラム**のテキスト値は、メールボックスの保留リストを更新することを示します。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="0d5ff-118">**削除**のテキスト値は、メールボックスの保持を削除することを示します。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0d5ff-119">備考</span><span class="sxs-lookup"><span data-stu-id="0d5ff-119">Remarks</span></span>

<span data-ttu-id="0d5ff-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0d5ff-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d5ff-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="0d5ff-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d5ff-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="0d5ff-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d5ff-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0d5ff-124">Schema name</span></span>  <br/> |<span data-ttu-id="0d5ff-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0d5ff-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d5ff-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0d5ff-126">Validation file</span></span>  <br/> |<span data-ttu-id="0d5ff-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0d5ff-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d5ff-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0d5ff-128">Can be empty</span></span>  <br/> |<span data-ttu-id="0d5ff-129">false</span><span class="sxs-lookup"><span data-stu-id="0d5ff-129">false</span></span>  <br/> |
   


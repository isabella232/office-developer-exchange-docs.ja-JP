---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: 要素では、開封確認をするかどうかを示す SuppressReadReceipts を抑制する必要があります。
ms.openlocfilehash: 794252da6b3e6b6e6f36181c1811a2a001bfaf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839630"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="38b31-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="38b31-103">SuppressReadReceipts</span></span>

<span data-ttu-id="38b31-104">**SuppressReadReceipts**要素を示す確認メッセージを抑制するかを読み取るかどうか。</span><span class="sxs-lookup"><span data-stu-id="38b31-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="38b31-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="38b31-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38b31-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="38b31-106">Attributes and elements</span></span>

<span data-ttu-id="38b31-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38b31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38b31-108">属性</span><span class="sxs-lookup"><span data-stu-id="38b31-108">Attributes</span></span>

<span data-ttu-id="38b31-109">なし。</span><span class="sxs-lookup"><span data-stu-id="38b31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38b31-110">子要素</span><span class="sxs-lookup"><span data-stu-id="38b31-110">Child elements</span></span>

<span data-ttu-id="38b31-111">なし。</span><span class="sxs-lookup"><span data-stu-id="38b31-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38b31-112">親要素</span><span class="sxs-lookup"><span data-stu-id="38b31-112">Parent elements</span></span>

<span data-ttu-id="38b31-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="38b31-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="38b31-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="38b31-114">Text value</span></span>

<span data-ttu-id="38b31-115">の**場合は true** 、 **SuppressReadReciepts**要素のテキスト値では、読み取り確認メッセージが抑制されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="38b31-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="38b31-116">**False**の値は、読み取り受信確認を送信者に送信されますを示します。</span><span class="sxs-lookup"><span data-stu-id="38b31-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="38b31-117">備考</span><span class="sxs-lookup"><span data-stu-id="38b31-117">Remarks</span></span>

<span data-ttu-id="38b31-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="38b31-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="38b31-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="38b31-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38b31-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="38b31-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38b31-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="38b31-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38b31-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38b31-122">Schema name</span></span>  <br/> |<span data-ttu-id="38b31-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="38b31-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38b31-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38b31-124">Validation file</span></span>  <br/> |<span data-ttu-id="38b31-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38b31-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38b31-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="38b31-126">Can be empty</span></span>  <br/> ||
   

